# trailmap

`trailmap` is a small Windower 4 addon for Final Fantasy XI. 
It draws an opaque black overlay and plots your movement into a simple trail, 
so each zone gradually becomes a personal breadcrumb map.

I originally wanted this app to help with Nyzul Isle Investigation 
but I've found it handy in other zones too.

## Install

1. Copy the `trailmap` folder into your Windower `addons` folder.
2. The main file should be `addons/trailmap/trailmap.lua`.
3. In game, run:

```text
//lua load trailmap
```

## Commands

```text
//tm toggle -- hides or shows 
//tm reset -- resets trail, places a new '+' at your current location
//tm clear -- clears current trail, keeps '+' at orginal location (starting location)
//tm center -- changes map view to start location while stay anchored to the origin.
//tm pos <x> <y>
//tm size <odd width> <odd height>
//tm scale <yalms-per-cell>
//tm opacity <0-255>


Feature:
Trailmap has a backtrack eraser feature. Default is turned on.
Backtracking on your trail will erase it.

//tm eraser [cells] -- Changes radius of your backtrack erasing. Default is '4'.
Smaller the number the closer you need to be to your trail for it to erase.  
//tm eraser turns eraser on/off.

 

//tm status -- debug
//tm test -- debug forces a simple text message at `40,80` to verify rendering.
//tm primtest --debug draws primitive test blocks;
//tm show clears test blocks and resumes the live map.

```

## Notes
- The live map is drawn with Windower primitives.
- The map projection is rotated and mirrored to match in-game movement.
- Backtracking near the previous trail erases it by default.

Produced and Directed by Talonn @Ragnarok 
Coded with AI: Codex and Gemini Code Assist.

