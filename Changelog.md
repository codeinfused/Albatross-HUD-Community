<div id="top"></div>

<!-- ABOUT ALBATROSS HUD -->
## Albatross HUD Change History

### 2.4.3
* Fixed a display bug causing the not-trustworthy space autopilot to not update.

### 2.4.1
* Introduced HOTAS stick and controller support using Lua setting bindings. See CodeInfused youtube video for how to set up.

### 2.3.1

### 2.2.2
* Added parameter hudTextColor for forcing HUD text color. Leave blank quotes for auto-color.
* Autopilot things.
* FIXED: Lua tab "time" command now works correctly.

### 2.2.1
* Added ALT+MMB for instant full-throttle. MMB cuts throttle to zero.
* Added atmospheric threshold on re-entry burn limiter to only cut throttle in 'deep space'.
* Reduced FPS lag issues over longer flights.
* Added my voice sound files to the repo with instructions on how to install.
* FIX: Align CLI tool when enabled in atmo used to set an invalid target vector.

### 2.2.0
* FIX: Language support on radar names for FR and DE.
* FIX: Landing mode and hover controls should work as expected again.
* FIX: Fuel tank names should no longer break the HUD.
* FIX: Added player mass and docked construct mass to total display ship mass and calcs.
* FIX: Entering seat while in space no longer engages landing mode.
* FIX: Added the Headlights hotkey (S:L) back in from default keybind.
* Improved braking calculations (thanks to AviatorHUD).
* Added basic space alignment commands in command line tools (align ::pos).
* Improved atmospheric entry and exit assistance (part of burn limiter function).
* Added button (AS:8) to toggle burn limiter while piloting.
* Added param option to hide the HUD reticles.
* Landing mode now engages brakes and kills throttle if speed under 500 (configurable).
* Improved underwater hover performance slightly.

### 2.1.2
* Added a param option for atmo speed limiter (default on). If on, this will limit your speed in atmosphere to 8% less than the ship's burn speed. In space, it will attempt to slow you down to under the burn speed before hitting the atmosphere (this will not work on moons).
* Added a param option to add a new flight mode toggle for ground-hover mode (default off). This mode essentially disables your airfoils and maxes hover height with auto-level.
* Added a hotkey (A+S:9) to toggle the Build Helper display (default off).

### 2.1.1
* Fixed AGG reading previous target instead of resetting target to current Base.
* Removed the voice command option from showing up erroneously.

### 2.1.0
* Added new HUD widget to support Antigravity display and control.
* Added param option to switch Brakes mode to a pure toggle control.
* Corrected max cruise speed in space.
* Increased default HUD scale.
* Added param option for ship to begin in Cruise mode instead of Throttle.
* Added param option for remote control units to freeze player movement or not.
