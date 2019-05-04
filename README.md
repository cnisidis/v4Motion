# v4Motion (blender addon)



Blender File Exchange Addon for vvvv (or just messing with skeletons)

The general idea is to simplify the huge loaded FBX files for simple skeletons and long duration movements which are causing oftenly frame dropping in vvvv

In order to keep it is as simple as it gets only the absolute positions of each joint are being exported in a file as raw data (bytes) with a short header which defines the block and few attributes.


There are three different file types with one extentsion (v4m) which correspond to different settings, for instance the first one (0) is only T (translation rotation) the second (1) is extended Translation and Rotation and the third (2) is T + Matrices.

The last one (Matrix - which is by the way the default setting) was aiming to replace the FBX file exporting for an ongoing project, but this is not probably the way since FBX files are storing relative Rotations and Translations on a current default state which is being defined on the header of each joint (or this is what I understood so far).

You may use it freely and change it according to your needs 


**Notes**

The addon is supporting both actions and NLA strips but it cant export all of them at once, so you have to export one strip at a time or the whole action instead


**recommended versions:**
- blender 2.79b
- vvvv beta 38.1


