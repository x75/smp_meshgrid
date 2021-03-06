hexgrid project
===============

a simulation and realtime monitor / interface to spatial structures. the structure is defined as a mesh which can be rendered and also serve as a structure to organize computing modules with spatial properties.

requirements
============

-   pygame
-   pyopengl
-   numpy, scipy - can also be installed with distribution tools
-   pyliblo - python wrapper for liblo OSC library
-   trimesh, meshpy - mesh libraries

``` example
pip3 install pygame pyopengl numpy scipy pyliblo trimesh pyzmq joblib meshpy
```

running scripts
===============

to run the demo go into the project directory

``` example
cd smp_meshgrid
```

trigrid\_display
----------------

then start the GL display with

``` example
python3 scripts/trigrid_display.py --width=1600 --height=900
```

trigrid
-------

this contains the model, and when running loads a mesh and sends vertex, edge and face information derived from model states to the display server. run it with

``` example
python3 scripts/trigrid.py
```

### trigrid modes

there is a few predfined meshes (hexagon, line, ...). the model can run on its own and it can be connected with the physical hexagon using libsensorimotor

then there are a few modes that serve as simple demo and starting points for extending the activation and coupling rules.

-   threshold crossing triggered activation with lateral coupled neighbors
-   TODO: random activation and isotropic propagation
-   TODO: liquid model

modules
=======

-   oscsrv
-   sensorimotor


misc
====

bla

