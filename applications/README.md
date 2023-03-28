# SentinelOne - STAR RULES

## Instalace 64bit aplikace

Doporučená závažnost: Low
```
RegistryKeyPath StartsWith Anycase "MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall" AND EventType = "Registry Key Create"```

## Instalace 32bit aplikace

Doporučená závažnost: Low
```
RegistryKeyPath StartsWith Anycase "RegistryKeyPath StartsWith Anycase "MACHINE\SOFTWARE\Wow6432Node\Microsoft\Windows\CurrentVersion\Uninstall" AND EventType = "Registry Key Create""```
