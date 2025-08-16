# Power Calligraphy
## Commands:
 
`0x100` - Input : Requires the player to press  after 1.0 beat.

 
`0x101<0> X` - Sets up the pattern

- 0 - 己 (onore)
- 1 - 力 (chikara)
- 2 - 寸 (sun)
- 3 - 心 (kokoro)
- 4 - レ (re)
- 5 - 、 (ten)
- 6 - つるニハ○○ムし (kao)
- 7 - 完 (The End)

`0x101<1> X` - Sets the next section of the pattern to be written (Numerical progression)

`0x102 X, Y` - Page Movement (by X and Y coordinates)

`0x103 X` - Next Page

- 0 - Normal
- 1 - Slow


`0x104 X` - Stroke type (What pressing  will do)
- 0x0 - 己
- 0x1 - 力 (Unused Stroke)
- 0x2 - 力
- 0x3 - 寸 (Stroke)
- 0x4 - 寸 (Dot)
- 0x5 - 心 (Stroke)
- 0x6 - 心 (Unused Upper Dot)
- 0x7 - 心 (Dot)
- 0x8 - レ
- 0x9 - 、
- 0xA - つるニハ○○ムし

`0x105 X, Y, Z` - Move Brush
- X - X position of the brush
- Y - Y position of the brush
- Z - "Depth" of the brush
	- 0 - Brush moves on the paper
	- 1 - Brush moves over the paper

`0x105<1> X` - Ready

- 0 - Stroke
- 1 - Dot

`0x105<2> X` - Color

- 0 - Normal
- 1 - Red

`0x105<3>` - Lift brush after doing a dot (used only by 寸)

`0x105<4>` - Ready Sound Effect (Press Down)

`0x105<5>` - Ready Sound Effect (Lift Up)

`0x106` - Hide Mini-Townfolk

`0x106<1> X` - Mini-Townfolk Animations

- 0 - Remove
- 1 - Default (Spawn)
- 2 - Fall Over
- 3 - Bow
- 4 - Kneel

## Subs:
*All subs except 0x72 through 0x74 are sync and must be called with* `sub`

`0x56` - 力 (Page)

`0x57` - 力

`0x58` - 己 (Page)

`0x59` - 己

`0x5A` - 寸 (Page)

`0x5B` - 寸

`0x5C` - 心 (Page)

`0x5D` - 心

`0x5E` - レ (Page)

`0x5F` - レ

`0x60` - 、 (Page)

`0x61` - 、

`0x62` - つるニハ○○ムし (Page)

`0x63` - つるニハ○○ムし

<ins>The following are in Swing</ins>

`0x64` - 力 (Leftover) (Page)

`0x65` - 力 (Leftover)

`0x66` - 己 (Leftover) (Page)

`0x67` - 己 (Leftover)

`0x68` - 寸 (Unused) (Page)

`0x69` - 寸 (Unused)

`0x6A` - 心 (Leftover) (Page)

`0x6B` - 心 (Leftover)

`0x6C` - レ (Leftover) (Page)

`0x6D` - レ (Leftover)

`0x6E` - 、 (Unused) (Page)

`0x6F` - 、 (Unused)

`0x70` - つるニハ○○ムし (Unused) (Page)

`0x71` - つるニハ○○ムし (Unused)

`0x72` - Power Calligraphy (Practice)

`0x73` - Power Calligraphy (Real Game)

`0x74` - Power Calligraphy (Skipped Practice)