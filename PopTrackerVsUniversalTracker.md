If this comparison is incorrect or incomplete, please [open an issue](https://github.com/Ixrec/ArchipelagoDocs/issues) or make a pull request.

### Fundamental Differences:

A PopTracker packs' UI is always images of the game's items or areas, typically with colored squares representing which locations are in logic.
<br>
vs
<br>
Universal Tracker's primary interface is a list of location names that are in-logic. An .apworld can optionally provide UT "map pages" that closely resemble a PopTracker pack, but most do not.

PopTracker can't display anything for a world until someone makes a PopTracker pack for it.
<br>
vs
<br>
Universal Tracker often just works on a new .apworld without the world dev doing any work to specifically support UT (unless/until that .apworld has logic options or logic-changing randomness)

PopTracker packs can be developed independently of the .apworld / world dev. In exchange, they require re-implementing all of the world's logic from scratch, so they can easily be wrong or go out of date after world updates.
<br>
vs
<br>
Universal Tracker reuses the .apworld's logic with minimal or no changes. In exchange, the quality of Universal Tracker support depends on the .apworld / world dev.

Universal Tracker's map pages are officially intended as a way to prototype PopTracker packs (although not all world devs use them that way). So in addition to the option of an .apworld containing all of its own map page data (what UT calls an "internal pack"), an .apworld can also be configured so that Universal Tracker will use an "external (PopTracker) pack" the user has already installed to display that world's map pages.

### Equivalent/Shared Features

Both UT and PopTracker:
- can display any number of maps/tabs implemented by the pack/world dev
- can display any number of red/green/gray squares on each map/tab, representing whether a location is in logic and has already been checked
- can display a single square for mutiple locations
- have a GUI for switching between maps/tabs
- can "auto-tab" to different maps/tabs based on AP datastorage
- support glitch/trick logic that turns squares yellow instead of green
- can generally be used without running the game, as long as the AP server is up
	- unless the poptracker pack relies on UAT and/or USB2SNES
- can show/hide locations based on whether they apply to the current game
	- UT relies on whether the location exists in the AP server slot it's connected to
	- poptracker relies on "visibility rules" written in the pack

### Other Significant Differences

- PopTracker can do manual tracking; Universal Tracker only does auto-tracking

- PopTracker can do auto-tracking via UAT and/or USB2SNES and/or Archipelago; Universal Tracker only uses Archipelago

- PopTracker packs may have multiple "variants"

- PopTracker has item panels. In fact, some PopTracker packs (or variants) are just for items.

- PopTracker has more options for how to handle event locations

- PopTracker has more visual customization:
  - each "layout" (typically item panel, map panel, etc) can choose colors, alignments, margins, sizes, and even child layouts
  - each square can specify its size, shape, border thickness
  - the tooltip/overlay of each square can specify its own text, font size, color, background color, alignment, custom images for checked/unchecked, etc

- Adding Universal Tracker map pages to an .apworld signficantly increases the .apworld's size. Some world devs even offer a map-less version of the .apworld for hosts that will only use it for generation and never see the map pages. In contrast, PopTracker packs are always separate from the corresponding .apworld.

### Help Wanted/Unknown:

- PopTracker has scout/bounce handlers, what do these do?
- does PopTracker have any features around AP hints? UT has some

### Docs/Support Links

PopTracker setup and user docs: https://github.com/black-sliver/PopTracker
<br>
PopTracker pack dev docs: https://github.com/black-sliver/PopTracker/tree/master/doc 
<br>
PopTracker Discord Server: https://discord.gg/WqA9bqMK

Universal Tracker channel on the AP Discord Server: https://discord.com/channels/731205301247803413/1367270230635839539
<br>
Universal Tracker world dev docs: https://github.com/FarisTheAncient/Archipelago/tree/tracker/worlds/tracker/docs
<br>
Universal Tracker "Integration Library"/examples thread: https://discord.com/channels/731205301247803413/1367996449270530080
