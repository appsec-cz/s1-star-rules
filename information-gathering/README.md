# SentinelOne - STAR RULES

## Pokus o získání hesel na uložené WiFi sítě

Doporučená závažnost: High
```
EndpointOS = "windows" AND EventType = "Process Creation" AND
TgtProcCmdLine Contains Anycase "netsh wlan show profile" AND
TgtProcCmdLine Contains Anycase "key=clear"
```

## Agerovaný seznam uživatelských jmen u kterých selhala autorizace ##

PowerQuery
```
event.category = 'logins' AND event.login.loginIsSuccessful = false 
| group NumberOfFailedAttempts = count(event.login.loginIsSuccessful=false) by event.login.userName, endpoint.name
| sort -NumberOfFailedAttempts
```
