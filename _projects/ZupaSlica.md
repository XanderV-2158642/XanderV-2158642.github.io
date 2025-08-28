---
layout: page
title: "ZupaSlica"
description: "An stl slicer, that produces G-code meant for ender3 style printers"
technologies: ["CPP", "Clipper", "ImGUI"]
featured: true
date: 2025-01-06
---

## Why

ZupaSlica is made in the context of the course Computational Fabrication at UHasselt. The goal was to create a slicer that is able to create G-code for manifold objects, printable on the ender3. 

## What can ZupaSlica do?

The slicer is capable of loading STL files and displaying them.
![ZupaSlica STL loaded](/assets/pictures/zupaslica_chopped.png)

When a file is loaded multiple settings can be adjusted for the print:
- Nozzle temperature
- Bed temperature
- Print speed
- Layer height
- Nozzle diameter
- Number of shells
- Number of roofs
- Number of floors
- Infill percentage
- Skirt
    - skirt lines
    - skirt height

These settings are used when slicing, and the sliced model can be seen on the right.
This panel gives an intersection of the model of a certain layer. The layer can be manipulated using the slider, and a seethrough plane moves through the model showing the intersection with the model.
![Gif that shows the utility of the slider and the plane moving through the model](/assets/gifs/zupaslica_chopped.gif)

Then the g-code can be exported and printed on your 3D printer!
