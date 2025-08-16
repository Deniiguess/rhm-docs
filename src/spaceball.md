# Spaceball (0x0)
## Commands:
`0x100 0xXX, Y` - Input
- X - Time in Ticks
    - 0x30 (Low ball)
    - 0x60 (High ball)
    - Any other changes the times before hitting and plays the high ball sfx
- Y - Object Type
	- 0 - Baseball
	- 1 - Rice ball
	- 2 - Alien

`0x101 X` - Change costume
- 0 - Normal
- 1 - Red Head
- 2 - Bunny

`0x102<X> Y, Z` - Camera
- X - Interpolation
    - 0 - Instant Zoom
    - 1 - Linear Zoom
	- 2 - Smooth Zoom
- Y - Predetermined Position
    - 0 to 0xB (4 is default)
        - 0 is close, 0xB is far
- Z - Time in ticks
    - Values in game: 0x18, 0x30, 0x60, 0x90, 0xC0, 0x120, 0x180, 0x240, 0x2A0

`0x103<X>` - Alien
- 0 - Opening Animation
- 1 - Closing Animation
- 2 - Gone

`0x104 X` - Unused Animation for the Alien
- 0 - dance00
- 1 - dance01

## Subs:
`0x56` - Nothing (Unused)

`0x57` - Spaceball (Practice)

`0x58` - Spaceball (Real Game)

`0x59` - Spaceball (Skipped Practice)