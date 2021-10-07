# godot-colorblindness

![](ishihara.png)

A colorblindness simulator to help you design for everyone.

If you like **godot-colorblindness**, please consider buying me a coffee:  
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/E1E53SKZF)

The color calculations I use are heavily based on:
* [Color Blindness Simulation Research](https://ixora.io/projects/colorblindness/color-blindness-simulation-research/)
* [Digital Video Colourmaps for Checking the Legibility of Displays by Dichromats](http://vision.psychol.cam.ac.uk/jdmollon/papers/colourmaps.pdf)
* [This page on color space transformation matrixes](http://www.brucelindbloom.com/index.html?WorkingSpaceInfo.html)
* [The wikipedia page on sRGB](https://en.wikipedia.org/wiki/SRGB)

The Godot Ishihara plate has been generated with [this tool](https://franciscouzo.github.io/ishihara/).

# Usage

- Install the plugin through Godot's AssetLib.
- Activate it from the Plugin menu (`AssetLib` => `Plugins` button).
- This adds a new control called `Colorblindness` under `CanvasLayer`. 
- Create a new `Colorblindness` control to it in your scene.
- Specify the `Type` property (eg. `Deuteranopia`).

Everything that renders under the control will appear tinted to match your selected color-blindness mode.

# Known issues

- Setting `Framebuffer Allocation` to `2D without Sampling` makes the addon unusable ([#4](https://github.com/paulloz/godot-colorblindness/issues/4)).

# Sample

The following sample shows normal vision, Protanopia, Deuteranopia, and Tritanopia (in that order).

![normal vision](https://i.imgur.com/utF2kHk.gif)
Normal vision

![Protanopia](https://i.imgur.com/mbzqc6e.gif)
Protanopia

![Deuteranopia](https://i.imgur.com/vHoA4UD.gif)
Deuteranopia

![Tritanopia](https://i.imgur.com/QPyvkxB.gif)
Tritanopia

