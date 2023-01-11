# SentinelOne - STAR RULES

## Použití lokálního admin účtu

Doporučená závažnost: Low
```
ObjectType = "LOGINS" and LoginIsSuccessful IS TRUE and UserName = "Administrator"
```

