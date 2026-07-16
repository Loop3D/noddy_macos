NODDY -- MACOS RUNTIME BUNDLE
================================

Just download the entire repository as a zip file, unzip it and 
run noddy.dmg by double clicking on it- everything it needs is in this folder

For full source code of this version see https://github.com/Loop3D/noddy_qt 
and for legacy codes see https://tectonique.net/noddy

Batch/CLI mode also works from here, e.g. from a Command Prompt/
PowerShell in this folder:

  open noddy.dmg somefile.his -block

Use open noddy.dmg -help for the full list of batch options.

This bundle was copied from a build of:
  noddy-code-r2-orig_src\noddy  (Qt5/MinGW64 build via its Makefile)

To refresh this bundle after rebuilding noddy, re-copy noddy from that build tree --


New Features
This port has allowed several new features to be added to the code:
- Clicked orientations on maps and sections now include x,y,z coordinates when saved to file
- Uniform grid of bedding orientations and lithology can be saved as cvs for whole top surface of map (Save Surface Orientations... menu item)
- Random 5-event history generator added (Random History menu item)
- Voxels above topo surface in block diagrams can now be rendered transparent (In Display Type Dialog).
- Gaussian noise can now be added to density and magnetic susceptibility at voxel level (In Geophysics Calculation Options)

To make noddy.app just use make
To make noddy.dmg, use make then /opt/local/libexec/qt5/bin/macdeployqt noddy.app -dmg
