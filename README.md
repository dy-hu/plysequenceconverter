# .Ply Sequence Converter
[Upgraded support from Stop Motion OBJ (Justin Jensen) ](https://github.com/neverhood311/Stop-motion-OBJ/wiki#quick-start)

> Stop Motion OBJ is a tool that lets you import a sequence of mesh files (.obj, .stl, or .ply), play them back in real time, then render them out to an animation. Each mesh may have a different vertex count, poly count, and even different UVs. This is especially useful for importing fluid simulations, for visualization of scientific data, and for rendering of 4D scan data.

### Stop Motion OBJ has been deprecated since Blender version 2.8.3

This .Ply Sequence converter plugin takes the .ply elements of the Stop Motion Obj, upgrading support for Blender 4.0+. 

> Stop Motion OBJ is able to import very complex mesh sequences that cannot fit in memory. Using [Streaming sequences](https://github.com/neverhood311/Stop-motion-OBJ/wiki#streaming), you can specify how many meshes to keep in memory at any given time and Stop Motion OBJ will automatically load and/or remove meshes so you don’t run out of memory.

# Gallery
| | | |
|:---:|:---:|:---:|
|[<img src="imgs/lee_perry_smith_256.gif">](https://github.com/neverhood311/Stop-motion-OBJ/wiki#gallery)|[<img src="imgs/mike_brondbjerg_s2g_neural_256.gif">](https://github.com/neverhood311/Stop-motion-OBJ/wiki#gallery)|[<img src="imgs/water_splash_256.gif">](https://github.com/neverhood311/Stop-motion-OBJ/wiki#gallery)|
|Lee Perry Smith \| [Infinite Realities](https://ir-ltd.net/) \| [AEONX](https://aeonx.com/)|Mike Brondbjerg \| [kultur.design](http://www.kultur.design/) \| [Twitter](https://twitter.com/mikebrondbjerg)|XC Engineering \| [XC Engineering](https://www.xceng.com/en/) \| [FLOW-3D](https://www.flow3d.com/)|
||||
|[<img src="imgs/frank_dsouza_256.gif">](https://github.com/neverhood311/Stop-motion-OBJ/wiki#gallery)|[<img src="imgs/day_107_256.gif">](https://github.com/neverhood311/Stop-motion-OBJ/wiki#gallery)|[<img src="imgs/day_109_256.gif">](https://github.com/neverhood311/Stop-motion-OBJ/wiki#gallery)|
|Franklyn D'souza \| [Twitter](https://twitter.com/franklynd/status/1231625663095934977)|Justin Jensen \| [Fourveo](https://www.researchgate.net/publication/325426062_Fourveo_Integration_of_4D_Animation_into_Conventional_3D_Animation_Workflows) \| [YouTube](https://www.youtube.com/channel/UCHnTdtUrB1L_1Xyid8tyZPg)|Justin Jensen \| [Fourveo](https://www.researchgate.net/publication/325426062_Fourveo_Integration_of_4D_Animation_into_Conventional_3D_Animation_Workflows) \| [YouTube](https://www.youtube.com/channel/UCHnTdtUrB1L_1Xyid8tyZPg)|


# Download & Install
To install, download the existing code as a folder, name it something descriptive. Make sure you have a .zip file, then open Blender and click Edit > Preferences... > Add-ons. Then click Install… and find the .zip file you previously downloaded. Once you’ve enabled the add-on, it should be ready to use immediately. You can enable it under the name "Point Cloud Sequence Importer."

# Quick Start Tutorial
<img src="imgs/cached_import_s2g_octree.gif" title="Quick Cached Sequence import">

Importing a .ply mesh sequence is easy:
1. Click File > Import > Mesh Sequence
1. Navigate to the folder where your mesh sequence is stored
1. In the File Name box, provide the first few letters of the name of one of your mesh files (prefix). Ensure that all files that you wish to import share this prefix
1. Click Select Folder and wait while your sequence is loaded
1. Click Object -> Set Origin -> Origin to Geometry
1. Alt-G to ensure object is centered
1. Scale your object to 0.2 for x,y,z so you can see it in the camera
1. Navigate to the Output section (should look like a printer) on the lower right, make sure your output is set to FFmpeg video
1. View -> Render Animation, then the output will be saved to the folder located in the output tab

Once it’s finished loading, you’re done!

# Acknowledgements
Special thanks to Justin Jensen for creating Stop Motion OBJ, and the Blender wiki docs for their descriptive documentation to help the migration of this to a higher version.
