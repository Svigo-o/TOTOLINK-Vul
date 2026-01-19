# TOTOLINK-Vul
Totolink 路由器漏洞复现与分析记录。

## 漏洞列表

| 目录 | 产品 | 接口/功能 | 参数 | 类型 |
| --- | --- | --- | --- | --- |
| [totolink-a3300r-password-cmd-injection](totolink-a3300r-password-cmd-injection) | A3300R | DDNS / `setDdnsCfg` | `password` | Command Injection |
| [totolink-a3300r-provider-cmd-injection](totolink-a3300r-provider-cmd-injection) | A3300R | DDNS / `setDdnsCfg` | `provider` | Command Injection |
| [totolink-a3300r-mode-cmd-injection](totolink-a3300r-mode-cmd-injection) | A3300R | Schedule / `setScheduleCfg` | `mode` | Command Injection |
| [totolink-a3300r-hour-cmd-injection](totolink-a3300r-hour-cmd-injection) | A3300R | Schedule / `setScheduleCfg` | `hour` | Command Injection |
| [totolink-a3300r--week-cmd-injection](totolink-a3300r-week-cmd-injection) | A3300R | Schedule / `setScheduleCfg` | `week` | Command Injection |
| [totolink-a3300r-rechour-cmd-injection](totolink-a3300r-rechour-cmd-injection) | A3300R | Schedule / `setScheduleCfg` | `recHour` | Command Injection |
