# BIA

Closed-source **Nuclear Option** BepInEx library. Source is not included.

Drop `BIA.Runtime_<version>.dll` into `BepInEx/plugins`. The **assembly name inside the file is `BIA.Runtime`** so existing `.baas` prefabs keep resolving.

Other mods should declare:

```
[BepInDependency("bia.runtime")]
```

BIA then lists those plugins on the left boot load bar, along with `BIARadar` / `BIAMfd` / `BIACountermeasures` / `BIAAirbrake` / `BIAGearHide`.

## Install

1. Install BepInEx for Nuclear Option.
2. Copy `BIA.Runtime_1.0.2.dll` into `BepInEx/plugins` (not a subfolder).
3. Remove any older `BIA.Runtime.dll` / `BIA.Runtime_*.dll` so only one copy loads.
4. Fully quit Steam (tray icon too), then launch.

Download the DLL from **Releases**. This repository does not ship source.

## License

Proprietary. All rights reserved. See `LICENSE`.
