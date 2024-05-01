---
layout: page
title: Demos
description: >-
    Demos page.
---

# List of demos for class

This page aggregates all demos shown in class.  A lot of these demos will be live coded in class to varying levels of success - these are the "working" versions of what is intended to be shown.

**Note**: these will mainly use the libraries from the Angel textbook - please see the [setup guide](setup.md) for how to get up and running with a local development environment!  

---

## WebGL Demos

These are all the WebGL-specific demos from class.  You can translate them to other libraries (e.g., three.js) - however they require some effort.  I have a few of the basics at the bottom of this page to get you started if you'd like to explore.

## 1 - Basic WebGL and Animation/Callbacks

* [Hello world - basic](hello-world-basic.html){:target="\_blank"}
* [Hello world - triangle](triangle.html){:target="\_blank"}
* [Square with different primitives](square.html){:target="\_blank"}
* [Sierpinski Gasket 1](gasket1.html){:target="\_blank"}
* [Sierpinski Gasket 2](gasket2.html){:target="\_blank"}
* [Sierpinski Gasket 3](gasket3.html){:target="\_blank"}
* [Sierpinski Gasket 4](gasket4.html){:target="\_blank"}
* [Sierpinski Gasket 5](https://efredericks.github.io/CIS367-ComputerGraphics/Chap3/gasket5.html){:target="\_blank"}
* [Circle (triangle fan)](triangle_circle.html){:target="\_blank"}
* [Shaded triangle](https://efredericks.github.io/CIS367-ComputerGraphics/demos/triangle-shade.html){:target="\_blank"}
* [jQuery callback](https://efredericks.github.io/CIS367-ComputerGraphics/demos/jqueryInput.html){:target="\_blank"}
* [Rotating Square](https://efredericks.github.io/CIS367-ComputerGraphics/Chap3/rotatingSquare1.html){:target="\_blank"}
* [Rotating Square 2](https://efredericks.github.io/CIS367-ComputerGraphics/Chap3/rotatingSquare2.html){:target="\_blank"}
* [Square](https://efredericks.github.io/CIS367-ComputerGraphics/Chap3/square.html){:target="\_blank"}
* [CAD 1](https://efredericks.github.io/CIS367-ComputerGraphics/Chap3/cad1.html){:target="\_blank"}
* [CAD 2](https://efredericks.github.io/CIS367-ComputerGraphics/Chap3/cad2.html){:target="\_blank"}

---

<!--
*in progress*

* [Metaballs](metaballs.html){:target="\_blank"}
  * Based on this tutorial: [Metaballs and WebGL](http://jamie-wong.com/2016/07/06/metaballs-and-webgl/){:target="\_blank"}

* Colors
* Cameras and lighting
* Primitives
  * Triangles
  * Squares
  * Polygons
* Sierpinski gasket 2D
* Sierpinski gasket 3D 
* Menger sponge
* Animation
* Picking
* User interfaces (via HTML)
* Images / Textures
* Model-View-Projection Examples (shear, etc.)
* Quaternions
* Meshes
* Perspectives
* Voronoi diagrams
* Ray tracing
* Slow particles
* Fast particles (or, let's GPU)
* three.js + Blender

--- 
-->

## Three.js Demos

* [Hello world - 2D (triangle)](hello-world-triangle.html){:target="\_blank"}
* [Hello world - 2D (rotating triangle)](hello-world-triangle-rotate.html){:target="\_blank"}
* [Hello world - 3D (rotating cube)](hello-world-cube.html){:target="\_blank"}

### Generative

* Voronoi
  * [Voronoi - Mouse Movement](voronoi-mouse.html){:target="\_blank"}
  * [Voronoi - Sine](voronoi-sin.html){:target="\_blank"}
  * [Voronoi - Full](voronoi-full.html){:target="\_blank"}
    * Based on this tutorial: [Cellular Noise](https://thebookofshaders.com/12/){:target="\_blank"}
* [Reactive audio visualizer](reactive-viz.html){:target="\_blank"} 
    * Based on this tutorial: [Creating an Interactive Spectrogram With Three.js and GLSL Shaders](https://calebgannon.com/2021/01/09/spectrogram-with-three-js-and-glsl-shaders/){:target="\_blank"}

## Blender Demos

### Set camera to top-down 2D view

*c/o: [Blender StackExchange](https://blender.stackexchange.com/questions/49197/how-to-get-camera-view-like-top-view){:target="\_blank"}*

1. Select camera in scene heirarchy
2. `Alt+g` (reset position)
3. `Alt+r` (reset rotation)
4. `g+z` (move along z-axis)

### Rotate camera around object (at origin)

1. Add an empty (axes)
2. Parent camera to empty
    * Click the empty 
    * Hold shift, grab camera, move onto empty
3. Animate empty

### Fluid simulation

* See: https://www.versluis.com/2022/06/creating-fluid-simulations-in-blender/

### Reuse node groups

* See: [Blender StackExchange](https://blender.stackexchange.com/questions/33576/how-do-you-import-a-compositing-node-set-up){:target="\_blank"}

## Unity Demos

* [Procedural Mesh Generation](https://catlikecoding.com/unity/tutorials/procedural-meshes/){:target="\_blank"}
* [2D Top Down Pixel Art RPG Crash Course](https://www.youtube.com/watch?v=7iYWpzL9GkM){:target="\_blank"}

## Old Demos

These demos are from a [prior incarnation of this course page](https://efredericks.github.io/CIS367-ComputerGraphics/){:target="\_blank"}.  I updated some of the Angel demos to work with newer browsers as some were broken. 
