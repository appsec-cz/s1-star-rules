# SentinelOne - STAR RULES

## Přidání vyjímky do firewallu

Doporučená závažnost: Low

```s1dvq
IndicatorName = "AddFirewallException" AND NOT SrcProcParentImagePath In Contains ("\Microsoft\EdgeUpdate\Install", "\Google\Update\Install")
```
