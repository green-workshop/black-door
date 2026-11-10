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

## Notes

- All graphics and sound are generated in code; there are no asset files.
- On integrated graphics the game lowers its render resolution automatically to hold frame rate.
- The setting is real but the events, characters and militia are fictional.
- The `.claude` folder holds a small preview server used during development. The game does not need it.
