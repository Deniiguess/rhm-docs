# Sneaky Spirits (0x2)
## Commands:
`0x100 X` - Input (Happens 1 beat after the command)
- X - Type
	- 0 - Normal
	- 1 - ???
	- 2 - ???
	- 3 - Practice (Doesn't laugh when you miss)

`0x101` - Draw Bow

`0x101<1> X, Y` - Slide Bow into View
- X - Starting Position
    - 0 - Standard position
    - 0xFA - Off screen (used in full games)
- Y - Time in Ticks
    - 0 - Already on screen
    - 0x60 - Takes 2 beats to arrive (used in full games)

`0x102 X` - Spirit Pops Up
- X - Position
    - 0 to 6

`0x102<1>` - Pause ghost mid-jump with arrow (Practice)

`0x102<2>` - Unpause ghost

`0x103` - Close Door

`0x104 X` - Spirit Height
- X - Height 
    - 0 to 0x100
    - 0 is totally hidden, 0x100 is totally up

`0x104<1> X` - Music Goes Quiet when Spirits go Lower
- 0 - Disable (Remix)
- 1 - Enable (Default)

`0x105 X` - Spirit Position
- 0 - Hit Zone (Temporarily stops ambience noise if hit)
- 1 - Behind the Fence

`0x105<1> X` - Unknown command
- 0 - Unknown, apparently unused
- 1 - Unknown

`0x106 X` - Butterflies (used in the short version)
- X - Amount 
    - Used Value: 6
    
`0x107` - Reset Speed

`0x107<1> X` - Game Slows Down when hitting a Spirit
- 0 - Disable (Remix)
- 1 - Enable (Default)


## Subs:
*All subs except 0x63 through 0x67 are sync and must be called with* `sub`

Sub names are derived from those found in RHRE.

`0x56` - Spirit - 8 beats

`0x57` - Spirit - 8 beats - Late fade-out

`0x58` - Spirit - 8 beats - Slow fade-out

`0x59` - Spirit - 8 beats - Fast fade-out

`0x5A` - Spirit - 8 beats - Fade-in

`0x5B` - Spirit - 8 beats - Fade-in fade-out

`0x5C` - Spirit - 8 beats - Fade-out fade-in

`0x5D` - Spirit - 8 beats - Odd beat

`0x5E` - Spirit - 8 beats - No sound

`0x5F` - Spirit - 7 beats

`0x60` - Spirit - 7 beats - Late fade-out

`0x61` - Spirit - 7 beats - Fast fade-out

`0x62` - Spirit - 7 beats - Fade-in

`0x63` - Skill Star (Timed to match Spirits)

`0x64` - Sneaky Spirits (Practice)

`0x65` - Sneaky Spirits (Real Game)

`0x66` - Sneaky Spirits 2 (Real Game)

`0x67` - Sneaky Spirits (Skipped Practice)

## Sub values:

| Sub | Beat 1 | Beat 2 | Beat 3 | Beat 4 | Beat 5 | Beat 6 | Beat 7 |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| 0x56 | 0x100 | 0x100 | 0x100 | 0x100 | 0x100 | 0x100 | 0x100 |
| 0x57 | 0x100 | 0x100 | 0x100 | 0x100 | 0xA0  | 0x50  | 0     |
| 0x58 | 0x100 | 0xC0  | 0x80  | 0x50  | 0x20  | 0     | 0     |
| 0x59 | 0x100 | 0xA0  | 0x50  | 0     | 0     | 0     | 0     |
| 0x5A | 0     | 0x20  | 0x40  | 0x70  | 0xA0  | 0xD0  | 0x100 |
| 0x5B | 0     | 0x40  | 0x80  | 0xA0  | 0x60  | 0x30  | 0     |
| 0x5C | 0x20  | 0x20  | 0x10  | 0x10  | 0x50  | 0xA0  | 0x100 |
| 0x5D | 0x20  | 0x100 | 0x10  | 0x100 | 0     | 0x100 | 0     |
| 0x5E | 0     | 0     | 0     | 0     | 0     | 0     | 0     |
| 0x5F | 0x100 | 0x100 | 0x100 | 0x100 | 0x100 | 0x100 | N/A   |
| 0x60 | 0x100 | 0x100 | 0x100 | 0xA0  | 0x50  | 0     | N/A   |
| 0x61 | 0x100 | 0xA0  | 0     | 0     | 0     | 0     | N/A   |
| 0x62 | 0     | 0x20  | 0x40  | 0x70  | 0xB0  | 0x100 | N/A   |
