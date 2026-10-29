# fishing-afk

Auto fishing for Blox Fruits. It casts, answers the bite, reels the fish in and casts again on its own, and moves you to a good spot by the water first. It comes with a small on/off panel.

## Run it

Have a fishing rod and bait selected, stand near the water and execute `fishing_afk.lua`.

- The panel on the left has an on/off switch, shows what the script is doing and counts your catches. Drag it by the title, `x` closes it.
- `L` turns it on and off too.
- It stops by itself, with a message on the panel, if you run out of bait or lose the rod.

## Executor functions needed

- `getgenv`
- `gethui` (optional, the panel falls back to the normal player GUI)

## Options

Set them before running, for example `getgenv().FishingAfkConfig = { AutoMove = false }`.

| Option | Default | What it does |
| --- | --- | --- |
| `StartOn` | `true` | start fishing as soon as it is executed |
| `Gui` | `true` | show the panel |
| `AutoMove` | `true` | move to a good spot by the water when needed, `false` to stay where you are |
| `SearchRadius` | `220` | how far (studs) it looks for a spot |
| `Perfect` | `true` | release the cast on a perfect throw |
| `AntiAfk` | `true` | keep the game from kicking you for being idle |
| `ToggleKey` | `Enum.KeyCode.L` | on/off key |

Scripting in Roblox can get an account banned. Use it at your own risk.

Obfuscated with Prometheus. Based on Prometheus by Elias Oelschner, https://github.com/prometheus-lua/Prometheus