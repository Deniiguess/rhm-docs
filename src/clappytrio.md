# The Clappy Trio (0x1)
## Commands:
`0x100 X` - Input
- X - Interval between claps in ticks
    - Input happens after twice as many ticks to account for middle Lion

`0x101 X` - Beat animation
- 0 - Normal
- 1 - Normal, usually used 1 beat for the ready stance

`0x101<1> X` - Set time before ready stance?
- X - Amount of beats before the ready stance
- Seems to have no effect?

`0x102<X>` - Ready stance
- 0 - Normal
- 1 - Determined

`0x103<X> Y` - Clap Animation
- X - Type
	- 0 - Normal
	- 1 - Normal (Unused)
- Y - Lion
	- 0 - Left Lion
	- 1 - Middle Lion
	- 2 - You (No Visible Effect)

`0x104 X` - Beat Animation Type
- 0 - Neutral Faces (Unused)
- 1 - Happy Faces

`0x105<X> "String"` - Sign
- X - Action
	- 0 - Sign drops down
	- 1 - Sign disappears
	- 2 - Sign is already down
- Y - String/Layout (Trio Timing!)
	- "Clap_ver_arrange.bflyt" (0x503074) - Trio Timing 🌵 (The Snappy Trio)
	- "Clap_ver_long.bflyt" (0x503122) - Trio Timing! (The Clappy Trio 2)
	- "Clap_ver_short.bflyt" (0x5031CD) - Trio Timing! (The Clappy Trio)
	- "Clap_ver_remix.bflyt"(0x509CDB) - Trio Timing 🍊 (Citrus Remix)

## Subs:
`0x56` - Clap (2.0 Beats Apart)

`0x57` - Clap (1.0 Beats Apart)

`0x58` - Clap (0.5 Beats Apart)

`0x59` - Clap (0.25 Beats Apart) (Unused)

`0x5A` - Clap (0.125 Beats Apart)

`0x5B` - Clap (0.75 Beats Apart)

`0x5C` - Clap (2.0 Beats Apart) (Unused)

`0x5D` - Clap (1.0 Beats Apart) (Unused)

`0x5E` - Clap (0.5 Beats Apart) (Unused)

`0x5F` - Clap (0.25 Beats Apart) (Unused)

`0x60` - The Clappy Trio (Practice)

`0x61` - The Clappy Trio (Real Game)

`0x62` - The Clappy Trio 2 (Real Game)

`0x63` - The Snappy Trio (Real Game)

`0x64` - The Clappy Trio (Skipped Practice)

