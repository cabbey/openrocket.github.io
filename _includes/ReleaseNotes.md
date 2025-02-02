Release Notes
=============

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-22.02.beta.02" class="a-no-format">
     OpenRocket 22.02.beta.02 (2022-03-26)
  </a>
</h2>

NOTE: Tube fin simulation is currently broken, and will be fixed in a future beta.

### New Features
* Check Java version at startup (requires Java 11)
* Opacity slider on appearance panel
* Export sim plots as PNG images

### Notable Bug Fixes
* Rocksim Import/Export
  * Corrected position offsets when importing and exporting (fixes issue 1164)
  * Corrected fin shape when importing (fixes issue 1220)
* Side boosters
  * Added stage selector for side boosters (fixes issue 1208)
  * Fixed simulation bug with side boosters (fixes issue 1210)
  * Eliminated warning when loading designs with boosters (fixes issue 1196)
  * Fixed Simulation Plot range with boosters (fixes issue 1228)
* More reliable creation of simulation when creating a new configuration (fixes issue 1163)
* No longer need to click on motor config to get flight data (fixes issue 1175)
* Motor database search more robust, especially for CTI (fixes issue 1174)
* More accurate and reliable simulation of fins on transitions (fixes issues 1173 and 1243)
* _plus other miscellaneous fixes_

### Other
* Set default color for all components to #BBBBBB, with Shine=30 (closes issue 1192)
* Update Mac installer style to more standard "drag app to Applications folder"

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-22.02.beta.01" class="a-no-format">
     OpenRocket 22.02.beta.01 (2022-02-25)
  </a>
</h2>

### Application
* Update to Java 11 
* Distributed as packaged installers

### New Rocket Design Capabilities
* **Pods**
* **Drop-off Boosters**
* **Rail buttons**
* **Attach freeform fins to nose cones and transitions**
* **Coefficient of Drag override**
* **Added Dave Cook's rocket component library**

### Staging Improvements
* Update CG correctly when stages are toggled
* Display stage names instead of numbers in Stage enable buttons
* Reported length reflects length of selected stages only
* More reliable deployment of booster stage recovery device
* Fixed booster tumbling behavior
* Eliminate exceptions during multi-stage simulation
* Improved accuracy of nose cone simulation

### Simulation Improvements
* Assorted CP calculation fixes
* Improved nose cone drag calculations
* Properly run all simulations when any design change is made
* Use actual burn time for determination of burnout event
* Improve mass calculation accuracy for motors
* Correct linear interpolation of motor CG
* Copy Simulation results to clipboard
* Report wind speed correctly
* Improved ground hit velocity calculations
* Run simulations all the way to the end
* No more warning if recovery device is deployed while motor is coasting

### Rocket Appearance
* Support rendering of transparent or translucent components
* Separate inside and outside color for tube components
* Separate left and right appearance for fin components

### User Interface
* Multi-select/copy/paste components in the tree
* Option to display rocket stability as percentage of length
* Improved layout on many windows and dialogs
* Now use "Export" to save to RKT format
* Improved File Dialog behavior
* Multi-select/delete motor configurations
* Improved UI appearance on Mac
* Motor Selection
  * Automatically open motor selection dialog when adding new motor configuation
  * Added checkbox to hide motors which are out of production
  * Highlight motor mount in rocket display when motor is selected
* Many improvements to freeform fin editor, including
  * More accurate insertion of new points
  * Highlight coordinates of selected point
  * Export fin profile to CSV file
  * Fixed scrolling and zooming
* Improvements to Photo Studio
  * Respond instantly to design changes
  * Settings saved per rocket
  * Settings layout improved
  * Settings values can now be entered via keyboard

### Misc
* Updated motor list to latest data from Thrustcurve.org
* Added additional fields to motors
* Disable fin-thickness warnings on phantom tubes
* Added warning message for phantom body tubes
* Updated print dialog to allow simulation control
* Improved Rocksim import
* Added or improved Spanish, Dutch, and simplified Chinese translations

..._plus many, many additional bug fixes and refinements_

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-15.03" class="a-no-format">
     OpenRocket 15.03 (2015-03-28)
  </a>
</h2>

OpenRocket now requires Java 1.7 for execution.

New Features

  * Experimental support for tube fins
  * Updated thrustcurves
  * Scriptable simulation extensions
  * Fin fillet mass
  * Better icons for different kinds of masses - altimeters, computers, etc.
  * Configurable default mach number
  * Improved preferences UI

Bug Fixes

  * Always use the correct filename extension when saving

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-14.11" class="a-no-format">
     OpenRocket 14.11 (2014-11-02)
  </a>
</h2>

New Features

  * Updated thrustcurves

Bug Fixes

  * Fixed a couple of bugs.

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-14.06" class="a-no-format">
     OpenRocket 14.06 (2014-06-25)
  </a>
</h2>

New Features

  * Klima motor textures
  * Added knots to windspeed and velocity units
  * Updated thrustcurves

Bug Fixes

  * Fixed annoying IndexOutOfBounds bug in tables.

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-14.05" class="a-no-format">
     OpenRocket 14.05 (2014-05-21)
  </a>
</h2>

New Features

  * Compute optimimum delay time when simulating
  * Display cg/mass overrides using icons in the component tree

Bug Fixes

  * Bug fixes in the motor selection dialog
  * Updated thrustcurves
  * Updated 3d libraries to 2.1.5

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-14.03" class="a-no-format">
     OpenRocket 14.03 (2014-03-20)
  </a>
</h2>

New Features

  * Photo Realistic 3d rocket renderer

Bug Fixes

  * Fixes to the flight configuration tab and motor selection dialog
  * Updated thrustcurves

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-13.11.2" class="a-no-format">
     OpenRocket 13.11.2 (2014-01-01)
  </a>
</h2>

Bug Fixes

  * Numerous bug fixes and usability improvements in the new
      flight configuration tab.
  * Fix couple of layout issues
  * Updated Spanish, French and Chinese translations

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-13.11.1" class="a-no-format">
     OpenRocket 13.11.1 (2013-11-15)
  </a>
</h2>

Bug Fixes

  * Added back the TubeConfiguration Configuration dialog
  * Seems the jogl update didn't happen in the 13.11 build.
  * Made the motor filter remember previous settings
  * Fixed various exceptions in flight configuration tables due to column reordering
  * Fixed NPE when deleting a configuration

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-13.11" class="a-no-format">
     OpenRocket 13.11 (2013-11-08)
  </a>
</h2>

New Features

  * Chinese translations
  * Replaced flight configuration dialog with more efficient configuration tab
  * Improved filtering in motor chooser dialog

Bug Fixes

  * Updated jogl to correct 3d problems on various platforms
  * Fixed NPE introduced by changes in Java 1.7.0_45-b18

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-13.09.1" class="a-no-format">
     OpenRocket 13.09.1 (2013-10-05)
  </a>
</h2>

This release contains a number of bug fixes, updated 3D JOGL
libraries.  Added preliminary thrustcurves for Aerotech C3 and D2 18mm
reloads.


<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-13.09" class="a-no-format">
     OpenRocket 13.09 (2013-09-08)
  </a>
</h2>

This release contains a number of bug fixes, updated 3D JOGL
libraries, and separates simulation edit and plot dialogs.

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-13.05" class="a-no-format">
     OpenRocket 13.05 (2013-05-04)
  </a>
</h2>

New Features

  * Added support for decals on rockets.  Added two new 3d views - 3d finished and 3d unfinshed.  Added support to export and
      apply decals (images) to rocket components.  Added ability to launch external graphics editor to edit decals and monitor
      file for writes to update the rocket view.
  * Added simulation of tumble recovery based on experimentation done by Sampo Niskanen.  This is particularly useful
      for low power staged flights.
  * Extended "motor configuration" concept to cover more properties.  The concept was renamed "Flight Configuration" and
      allows the user to override stage separation, recovery deployment, and motor ignition per flight configuration.
      These configurations are stored in the ork file with each component.  If no override is specified then the user specified
      default is used (set in the component edit dialog).  The flight configuration dialog was reworked to make it more
      usable.  The user selects the configuration in a drop down with buttons for "add", "delete" and "rename".  After selecting
      the configuration, the tabbed area below allows the user to change the configuration for this simulation.
  * Allow simulation of stages without a motor.  Users in the past have attempted to simulate separate recovery of payload
      and booster by tricking OpenRocket using a dummy motor with trivial thrust curve.  Now the user does not need to do this.
      There is an example of this provided in TARC Payloader.ork and Boosted Dart.ork
  * Simulate recovery of boosters.  The simulation engine will create new FlightDataBranches for each stage after
      separation.  The data for the boosters begins at t=separation.  The simulation plot allows the user to select
      which stage's data to show (or all).
  * Modified the zoom and pan controls in the simulation plot.  Added zoom in, out, and reset buttons.  Added
      scroll with mouse wheel.  If the alt key is used with either of these, only the domain is zoomed.  Richard
      contributed a more logical mouse controlled zoom - right click and drag will zoom (either domain, range or both).


<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-12.09.1" class="a-no-format">
     OpenRocket 12.09.1 (2012-06-28)
  </a>
</h2>

Bug-fix release for 12.09, fixing numerous bugs.  Only new feature is
the possiblity to automatically open the latest design file on startup
(in Edit -> Preferences -> Options).


<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-12.09" class="a-no-format">
     OpenRocket 12.09  (2012-09-16)
  </a>
</h2>

Numerous new features by many contributors

- 3D rocket design view
- Component Presets
- Custom expressions in simulations
- Printing for centering ring and clustered centering ring components.
- Support simple arthmatic in dimension entry
- Support deploying recovery device at stage separation
- Support for fractional inches (1/64) for unit length
- Added preference for windspeed units separately
- Added "most recently used files" in File Menu.
- Improved printed accurracy in fin marking guide
- Calibration rulers added to printed templates
- Translations in Czech and Polish, numerous updates


<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-12.03" class="a-no-format">
     OpenRocket 12.03  (2012-03-17)
  </a>
</h2>

In this release the version numbering scheme has been changed to be
"YY.MM" indicating the year and month of the release.

Enhancements in the desktop version include saving designs in RKT
format thanks to Doug Pedrick, freeform fin set import from images by
Jason Blood, configurable stage separation events, guided help tours
and displaying the computed motor designation class.  The application
has also been translated to Italian by Mauro Biasutti and Russian by
the Sky Dart Team.

This also marks the first release for Android devices.  In this first
release you can open files and examine existing simulations, stability
data and motor files.  The Android port is thanks to work by Kevin
Ruland.


<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-1.1.9" class="a-no-format">
     OpenRocket 1.1.9  (2011-11-24)
  </a>
</h2>

This release calculates rocket flight in real-world coordinates and
takes into account geodetic effects (including coriolis effect) thanks
to work by Richard Graham.  Printing of transitions, nose cone
profiles and fin marking guides is available thanks to Doug Pedrick.
It also contains some usability features and bug fixes.

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-1.1.8" class="a-no-format">
     OpenRocket 1.1.8  (2011-08-25)
  </a>
</h2>

This release contains bug fixes to the optimization methods.
It also contains a workaround to a JRE bug that prevents running
OpenRocket on Java 7.

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-1.1.7" class="a-no-format">
     OpenRocket 1.1.7  (2011-08-12)
  </a>
</h2>

This release contains automatic rocket design optimization
functionality.  However, be cautious when using it and take the
results with a grain of salt.

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-1.1.6" class="a-no-format">
     OpenRocket 1.1.6  (2011-07-22)
  </a>
</h2>

Internationalization support thanks to work by Boris du Reau and
translations by Tripoli Spain, Tripoli France and Stefan Lobas
(ERIG e.V.).  The release also contains rocket design scaling support
and numerous bug fixes.

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-1.1.5" class="a-no-format">
     OpenRocket 1.1.5  (2011-06-10)
  </a>
</h2>

Removed native printing support.  Printing is now handled via PDF
viewer, which should make printing much more reliable and less
bug-prone.

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-1.1.4" class="a-no-format">
     OpenRocket 1.1.4  (2011-03-05)
  </a>
</h2>

Initial printing support by Doug Pedrick, and various bug fixes.

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-1.1.3" class="a-no-format">
     OpenRocket 1.1.3  (2010-10-06)
  </a>
</h2>

Support for drag-drop moving and copying of components.  Fixes a
severe bug in the undo system.

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-1.1.2" class="a-no-format">
     OpenRocket 1.1.2  (2010-09-07)
  </a>
</h2>

Fixes a severe bug that prevented adding stages to rockets.

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-1.1.1" class="a-no-format">
     OpenRocket 1.1.1  (2010-09-03)
  </a>
</h2>

Major rewrite of the simulation code, enhanced support for thrust
curve loading and selection, faster startup time and bug fixes.

Old simulation listeners are incompatible with this release.

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-1.1.0" class="a-no-format">
     OpenRocket 1.1.0  (2010-03-21)
  </a>
</h2>

Support for loading RockSim rocket design files (.rkt) thanks to
Doug Pedrick.

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-1.0.0" class="a-no-format">
     OpenRocket 1.0.0  (2010-03-10)
  </a>
</h2>

Added numerous new motor thrustcurves from thrustcurve.org, and fixed
a few more bugs.

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-0.9.6" class="a-no-format">
     OpenRocket 0.9.6  (2010-02-17)
  </a>
</h2>

Updated aerodynamic calculation methods to be more in line with the
Barrowman method and enhanced simulation time step selection.  Fixed
numerous bugs.

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-0.9.5" class="a-no-format">
     OpenRocket 0.9.5  (2009-11-28)
  </a>
</h2>

Fixed a serious defect which prevented adding a tube coupler and
centering ring on the same body tube.  Other minor improvements.

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-0.9.4" class="a-no-format">
     OpenRocket 0.9.4  (2009-11-24)
  </a>
</h2>

Added through-the-wall fin tabs, attaching components to tube
couplers, material editing and automatic update checks, and fixed
numerous of the most commonly occurring bugs.

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-0.9.3" class="a-no-format">
     OpenRocket 0.9.3  (2009-09-01)
  </a>
</h2>

Numerous bug fixes and enhancements including data exporting, showing
flight events in plots, example rocket designs, splitting clustered
inner tubes and automated bug reporting.

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-0.9.2" class="a-no-format">
     OpenRocket 0.9.2  (2009-07-13)
  </a>
</h2>

Fixed imperial unit conversions.  Significant UI enhancements to the
motor configuration edit dialog, motor selection dialog and file
open/save.

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-0.9.1" class="a-no-format">
     OpenRocket 0.9.1  (2009-06-09)
  </a>
</h2>

Bug fixes to file dialog and saving; initial support for cut/copy/paste
of simulations.

<hr/>

<h2>
  <a href="https://github.com/openrocket/openrocket/releases/tag/release-0.9.0" class="a-no-format">
     OpenRocket 0.9.0  (2009-05-24)
  </a>
</h2>

Initial release.
