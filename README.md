# COOLmeDOWN
A daemon for Pokémon Go ~~users~~ spoofers, that monitors your clipboard for coordinates, showing a notification with cooldown time and distance whenever you copy a coordinate.

![](example.gif)

## Pre-Requisites

This uses libnotify and gtk3, so it's mostly oriented at Gnome users or any gtk-based DE.

**System Requisites** _(most likely already installed if you're an Ubuntu/Debian user or use Gnome as your DE)_:

- `python3`
- `python3-gi`
- `python-gobject`
- `libnotify`

**Python Libraries:**

        pip install -r requirements.txt

That's it.

**No Windows support!**, sorry. _Shouldn't be hard to port tho', give a try and submit a PR!_ :grin:

## How to "install".

Just run the script `COOLmeDOWN` and leave it running on the background.

Or, even better, add it to your startup applications and it'll work as a daemon.

## Extras

- **CALCyourCLOCK**: outputs cooldown time by passing coordinate as arguments.

- **CLOSEmeUP**: compares a single coordinate with a list of coordinates (e.g.: a list of nests) and prints the ones that are less than 120m away, by decrescent time order.


## TODO:

- Refactor everything into one single file (I was a noobie at the time).

- Make it into a proper Class so it can be easily imported and used in other projects.

- Make it compatible with Windows (I'm not doing it).