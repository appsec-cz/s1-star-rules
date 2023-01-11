# SentinelOne - STAR RULES

## Pokus o získání hesel na uložené WiFi sítě

Doporučená závažnost: High
```
EndpointOS = "windows" AND EventType = "Process Creation" AND
TgtProcCmdLine Contains Anycase "netsh wlan show profile" AND
TgtProcCmdLine Contains Anycase "key=clear"
```
