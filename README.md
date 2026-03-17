# TOTOLINK-Vul
Totolink 路由器漏洞挖掘与验证分析记录。

## 漏洞列表

| 目录 | 产品 | 接口/功能 | 参数 | 类型 |
| --- | --- | --- | --- | --- |
| [totolink-a3300r-password-cmd-injection](totolink-a3300r-password-cmd-injection) | A3300R | DDNS / `setDdnsCfg` | `password` | Command Injection |
| [totolink-a3300r-provider-cmd-injection](totolink-a3300r-provider-cmd-injection) | A3300R | DDNS / `setDdnsCfg` | `provider` | Command Injection |
| [totolink-a3300r-mode-cmd-injection](totolink-a3300r-mode-cmd-injection) | A3300R | Schedule / `setScheduleCfg` | `mode` | Command Injection |
| [totolink-a3300r-hour-cmd-injection](totolink-a3300r-hour-cmd-injection) | A3300R | Schedule / `setScheduleCfg` | `hour` | Command Injection |
| [totolink-a3300r-week-cmd-injection](totolink-a3300r-week-cmd-injection) | A3300R | Schedule / `setScheduleCfg` | `week` | Command Injection |
| [totolink-a3300r-rechour-cmd-injection](totolink-a3300r-rechour-cmd-injection) | A3300R | Schedule / `setScheduleCfg` | `recHour` | Command Injection |
| [totolink-a3300r-dhcp-mtu-cmd-injection](totolink-a3300r-dhcp-mtu-cmd-injection) | A3300R | WAN / `setWanCfg` | `dhcpMtu` | Command Injection |
| [totolink-a3300r-ttl-way-cmd-injection](totolink-a3300r-ttl-way-cmd-injection) | A3300R | WAN / `setWanCfg` | `ttlWay` | Command Injection |
| [totolink-a3300r-lcp-echo-enable-cmd-injection](totolink-a3300r-lcp-echo-enable-cmd-injection) | A3300R | WAN / `setWanCfg` | `lcpEchoEnable` | Command Injection |
| [totolink-a3300r-pppoe-service-name-cmd-injection](totolink-a3300r-pppoe-service-name-cmd-injection) | A3300R | IPv6 / `setIpv6Cfg` | `pppoeServiceName` | Command Injection |
| [totolink-a3300r-pppoe-mtu-cmd-injection](totolink-a3300r-pppoe-mtu-cmd-injection) | A3300R | IPv6 / `setIpv6Cfg` | `pppoeMtu` | Command Injection |
| [totolink-a3300r-enable-cmd-injection](totolink-a3300r-enable-cmd-injection) | A3300R | TR-069 / `setTr069Cfg` | `enable` | Command Injection |
| [totolink-a3300r-url-cmd-injection](totolink-a3300r-url-cmd-injection) | A3300R | TR-069 / `setTr069Cfg` | `url` | Command Injection |
| [totolink-a3300r-user-cmd-injection](totolink-a3300r-user-cmd-injection) | A3300R | TR-069 / `setTr069Cfg` | `user` | Command Injection |
| [totolink-a3300r-inform-enable-cmd-injection](totolink-a3300r-inform-enable-cmd-injection) | A3300R | TR-069 / `setTr069Cfg` | `informEnable` | Command Injection |
| [totolink-a3300r-interval-cmd-injection](totolink-a3300r-interval-cmd-injection) | A3300R | TR-069 / `setTr069Cfg` | `interval` | Command Injection |
| [totolink-a3300r-stun-enable-cmd-injection](totolink-a3300r-stun-enable-cmd-injection) | A3300R | TR-069 / `setTr069Cfg` | `stunEnable` | Command Injection |
| [totolink-a3300r-stun-server-addr-cmd-injection](totolink-a3300r-stun-server-addr-cmd-injection) | A3300R | TR-069 / `setTr069Cfg` | `stunServerAddr` | Command Injection |
| [totolink-a3300r-stun-port-cmd-injection](totolink-a3300r-stun-port-cmd-injection) | A3300R | TR-069 / `setTr069Cfg` | `stunPort` | Command Injection |
| [totolink-a3300r-stun-max-alive-cmd-injection](totolink-a3300r-stun-max-alive-cmd-injection) | A3300R | TR-069 / `setTr069Cfg` | `stunMaxAlive` | Command Injection |
| [totolink-a3300r-stun-min-alive-cmd-injection](totolink-a3300r-stun-min-alive-cmd-injection) | A3300R | TR-069 / `setTr069Cfg` | `stunMinAlive` | Command Injection |
| [totolink-a3300r-stun-user-cmd-injection](totolink-a3300r-stun-user-cmd-injection) | A3300R | TR-069 / `setTr069Cfg` | `stun_user` | Command Injection |
| [totolink-a3300r-stun-pass-cmd-injection](totolink-a3300r-stun-pass-cmd-injection) | A3300R | TR-069 / `setTr069Cfg` | `stun_pass` | Command Injection |
