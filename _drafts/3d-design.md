---
layout: post
title:  "3D design tools"
categories: CAD 3dprinting
---

Autodesk's [Tinkercad](https://www.tinkercad.com/) is a great way to get started, there are many interactive tutorials included. While being simple, it still allows sophisticated designs.
Tinkercad runs in your browser using WebGL, computations are performed on Autodesk's servers. The design is stored there as well, but it is possible to download `.STL` files.

A more advanced free tool is Autodesk [123D Design](http://www.123dapp.com/design). This is used for the Adafruit 3D printing designs for example.


## Open Source CAD Software

I prefer open source software, popular choices are [FreeCAD](http://www.freecadweb.org/) and [OpenSCAD](http://www.openscad.org/).

### OpenSCAD

OpenSCAD designs are written in its own scripting language, which compiles to the actual design.
This has the major advantage that you can easily build repeated structures. Edit properties without having to move the mouse to the precise value is much easier for me.
Keeping designs in version control and viewing differences between versions is much easier too.

There is a rendered preview in the GUI, but it does not allow editing objects from the visualization. You can [use an external editor with OpenSCAD](http://en.wikibooks.org/wiki/OpenSCAD_User_Manual/Using_an_external_Editor_with_OpenSCAD).

The user manual was not suitable for getting started when I read it, I recommend [this four article series](http://www.tridimake.com/2014/09/how-to-use-openscad-tricks-and-tips-to.html).

### FreeCAD

Quoting the FreeCAD wiki,

> FreeCAD makes heavy use of all the great open-source libraries that exist out there in the field of Scientific Computing. Among them are OpenCascade, a powerful CAD kernel, Coin3D, an incarnation of Open Inventor, Qt, the world-famous UI framework, and Python, one of the best scripting languages available.

[Python scripting FreeCAD](http://www.freecadweb.org/wiki/index.php?title=Python_scripting_tutorial)
