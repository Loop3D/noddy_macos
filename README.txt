NODDY -- MACOS RUNTIME BUNDLE
================================

Just download the entire repository as a zip file, unzip it and 
run noddy.dmg by double clicking on it- everything it needs is in this folder

For full source code of this version see https://github.com/Loop3D/noddy_qt 
and for legacy codes see https://tectonique.net/noddy

Batch/CLI mode also works from here, e.g. from a console in this folder:

  open noddy.dmg fold_tilt_fault.his -block

Use open noddy.dmg -help for the full list of batch options.


New Features
This port has allowed several new features to be added to the code:
- Clicked orientations on maps and sections now include x,y,z coordinates when saved to file
- Uniform grid of bedding orientations and lithology can be saved as cvs for whole top surface of map (Save Surface Orientations... menu item)
- Random 5-event history generator added (Random History menu item)
- Voxels above topo surface in block diagrams can now be rendered transparent (In Display Type Dialog).
- Gaussian noise can now be added to density and magnetic susceptibility at voxel level (In Geophysics Calculation Options)

To make noddy.app just use make
To make noddy.dmg, use make then /opt/local/libexec/qt5/bin/macdeployqt noddy.app -dmg


Qt distribution
Qt is used to build the GUI for this code. Distribution of Qt libraries for Open Source codes is allowed as long as the source code for the Qt libraries is made available (here https://download.qt.io/). The Qt code is ditributed under a LGPLv3 license lgpl-3.0.

Source Code
Full source code available here: https://github.com/Loop3D/noddy_qt/

Help
Manuals for legacy version and other resources can be found here: https://tectonique.net/noddy
