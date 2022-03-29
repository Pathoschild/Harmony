**This is a custom fork of Harmony 2.2.1 used by the Stardew Valley community.** It's bundled with
[SMAPI](https://github.com/Pathoschild/SMAPI) automatically. See
[pardeike/Harmony](https://github.com/pardeike/Harmony) for documentation and usage.

This fork is identical to the official version, with two changes:

* Generated method names include the patching Harmony IDs to help troubleshoot error logs:

  ```c#
  // with original Harmony
     at StardewValley.Farm.resetLocalState_Patch1(Object )

  // with fork
     at StardewValley.Farm.resetLocalState_PatchedBy<Pathoschild.SmallBeachFarm>(Object )
  ```

* The `0Harmony.dll` no longer has Mono.Cecil and MonoMod merged into it. This fixes some of their
  types being available to mods, and avoids compile errors in SMAPI since it uses Mono.Cecil too.

Here's a [list of changes](https://github.com/Pathoschild/Harmony/compare/v2.2.1.0...fork) in the
forked version.
