NODDY -- WINDOWS RUNTIME BUNDLE
================================

Just download the entire respository as a zip file, unzip it and 
double-click noddy.exe -- everything it needs is in this folder
(Qt5 DLLs + platforms\qwindows.dll), no separate Qt or MSYS2 install
required on the target machine. Verified to launch standalone with a
clean PATH.

For full source code of this version see https://github.com/Loop3D/noddy_qt 
and for legacy codes see https://tectonique.net/noddy

Batch/CLI mode also works from here, e.g. from a Command Prompt/
PowerShell in this folder:

  noddy.exe somefile.his -block

See -help for the full list of batch options.

This bundle was copied from a build of:
  noddy-code-r2-orig_src\noddy  (Qt5/MinGW64 build via its Makefile)

To refresh this bundle after rebuilding noddy.exe, re-copy noddy.exe
plus the *.dll files and platforms\qwindows.dll from that build tree --
see that project's user.txt for the full verified dependency list and
how to regenerate it (windeployqt or `ldd noddy.exe`) if Qt/MinGW
versions change.

New Features
This port has allowed several new features to be added to the code:
- Clicked orientations on maps and sections now include x,y,z coordinates when saved to file
- Uniform grid of bedding orientations and lithology can be saved as cvs for whole top surface of map (Save Surface Orientations... menu item)
- Random 5-event history generator added (Random History menu item)
- Voxels above topo surface in block diagrams can now be rendered transparent (In Display Type Dialog).
- Gaussian noise can now be added to density and magnetic susceptibility at voxel level (In Geophysics Calculation Options)

