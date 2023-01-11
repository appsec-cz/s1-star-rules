# SentinelOne - STAR RULES

## Remote Desktop - pokusy o exploit (BlueKeep)

Doporučená závažnost: High
```
IndicatorName = "MaliciousRDPConnection"
```

## RDP, SSH - chybné přihlášení

Doporučená závažnost: Medium
```
ObjectType = "logins" AND LoginIsSuccessful Is false AND LoginType = "NETWORK"
```

