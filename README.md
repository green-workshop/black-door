# BLACK DOOR

A one-level first-person shooter that runs in the browser. You are one of four SAS troopers defending the Prime Minister and 10 Downing Street against an armed militia attempting a coup.

**Play it:** https://green-workshop.github.io/black-door/

The whole game is a single file, [`index.html`](index.html). Download it and double-click it, or open the link above. It needs an internet connection to load the Three.js engine, and a desktop browser with a keyboard (Chrome or Edge recommended). There are no touch controls, so it does not work on phones.

## The mission

1. Take position at the barricade.
2. Hold the Whitehall gates when the militia break through.
3. Fight on two fronts when the west wall is breached.
4. Fall back inside Number 10 and defend the house.
5. Escort the Prime Minister to the secure room.
6. Hold until the relief force arrives.
7. Walk the Prime Minister out to the extraction vehicle.

Checkpoints are saved at each stage. Cars, fuel drums, windows, street lamps, chandeliers and furniture can all be destroyed.

## Controls

| Action | Keys |
| --- | --- |
| Move | `W` `A` `S` `D` |
| Look | Mouse, or arrow keys |
| Fire | Left mouse button, or `E` |
| Aim down sights | Hold right mouse button, or `X` to toggle |
| Sprint / jump / crouch | `Shift` / `Space` / `C` |
| Reload | `R` |
| Switch weapon | `1` `2` `Q` |
| Grenade / knife | `G` / `V` |
| Interact, pick up | `F` |
| Look sensitivity | `[` `]` |
| Pause (then quit to menu) | `Esc` |

## How it was made

This game is a demo of what a single prompt can produce. It was built by Claude Fable 5.2 (Anthropic), working in Claude Code, in one session. All the code in this repository was written by the model.

The opening prompt, verbatim:

> I'd like you to create a first person shooter based on Call Of Duty.  So i want game play and artwork to be very close to it.\
> I only want one level. the level and story behind it is as follows:\
> the user is assigned to protect the PM and 10 downing street.\
> the user is part of a team of 4 SAS. a threat is anticipated, a militia who intend perform a coup.  it's the users job to protect the PM from the threat.  Use street as well and the inside of the building as playable world. destruction of certain element is encouraged.\
> If this could be a single page app the better, but the game itself is priority.\
> Do you understand or have any questions?

The model replied with a short plan and five questions, each with a suggested default:

1. Single file or small folder? (A single file loading Three.js from a CDN needs an internet connection.)
2. Length and difficulty? (About 10–15 minutes, moderate, with checkpoints.)
3. Weapons? (Assault rifle, sidearm, grenades, and enemy weapons to pick up.)
4. Time of day? (Dusk or night with rain.)
5. Sound? (Synthesised effects, with subtitles instead of voice acting.)

The answer, verbatim:

> 1, internet connection is assumed.\
> 2) that's fine\
> 3) sounds great\
> 4) yep go with what you feel best\
> 5) please
>
> go

That exchange produced the playable game. Three short follow-ups came afterwards: a way to quit to the menu, the trackpad and keyboard-only controls, and publishing it here.

## Notes

- All graphics and sound are generated in code; there are no asset files.
- On integrated graphics the game lowers its render resolution automatically to hold frame rate.
- The setting is real but the events, characters and militia are fictional.
- The `.claude` folder holds a small preview server used during development. The game does not need it.
