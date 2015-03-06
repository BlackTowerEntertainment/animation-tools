Three.js - Animation Viewer
====================================
By: [Black Tower Entertainment](http://blacktowerentertainment.com/blog/)

Maya THREE.js exporter supporting static and animated meshes. The exporter is composed of
two files: threeJsFileTranslator.py and ThreeJsExportScript.mel. Place the Python file in
the Maya plug-ins/ folder. Place the MEL script in the Maya scripts/ folder. From Maya load
the exporter from the plug-ins window.
 
Exports Maya models to Three.js' ASCII JSON format.  Currently supports exporting the following:

- Vertices
- Faces
- Normals
- UV sets
- Material indices
- Vertex colors
- Bones
- Animations
- Skin Weights and Indices


Version 1.1
====================
[Black Tower Entertainment](http://blacktowerentertainment.com/blog/)

Installation
-------------------------

Copy the scripts and plug-ins folders to the appropriate maya folder, where `maya-version` is your current version of Maya (eg. 2013-x64).

- Windows: `C:\Users\username\Documents\maya\maya-version`
- OSX: `~/Library/Preferences/Autodesk/maya/maya-version`
- Linux: `/usr/autodesk/userconfig/maya/maya-version`

After that, you need to activate the plugin.  In Maya, open `Window > Settings/Preferences > Plug-in Manager` and enable the checkboxes next to `threeJsFileTranslator.py`.

Usage
-------------------------

1. Select the mesh only, not including the rig, joints or IKs.
2. Go to File > Export Selection.
3. Under Files of Type menu, select ‘THREE.js w/ Animations’.
4. Under the Mesh options, check ‘Skin Weights’.
5. Under the Animation options, check ‘Animations’.
6. Click export.

NOTE: The exported has only been tested up to Maya 2012. The exported may not be supported by later versions of Maya. 