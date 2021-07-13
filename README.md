**This is a custom fork of Harmony used by the Stardew Valley community.** It's bundled with
[SMAPI](https://github.com/Pathoschild/SMAPI) automatically. See
[pardeike/Harmony](https://github.com/pardeike/Harmony) for documentation and usage.

This fork is identical to Harmony 2.0.1, except that generated method names include the patching
Harmony IDs to help troubleshoot error logs:

```c#
// with original Harmony
   at StardewValley.Farm.resetLocalState_Patch1(Object )
   at StardewValley.GameLocation.<resetForPlayerEntry>b__219_0()
   ...

// with fork
   at StardewValley.Farm.resetLocalState_PatchedBy<Pathoschild.SmallBeachFarm>(Object )
   at StardewValley.GameLocation.<resetForPlayerEntry>b__219_0()
   ...
```

Here's a [list of changes](https://github.com/Pathoschild/Harmony/compare/v1.2.0.1...fork) in the
forked version.
