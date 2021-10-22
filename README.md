# harp-screenFix

automator keyboard shortcut to fix external "snow" screen on macbook air in clamshell mode when using kvm

## installation
1. Install [display manager](https://github.com/univ-of-utah-marriott-library-apple/display_manager#download)
2. Copy harp-Screenfix.workflow from this repo to ~/Library/Services.  Or alternately, [set up the workflow](https://developer.apple.com/library/archive/documentation/LanguagesUtilities/Conceptual/MacAutomationScriptingGuide/MakeaSystem-WideService.html) manually using display manager commands noted in history.md.

3. Assign a [non-conflicting](https://support.apple.com/guide/mac-help/if-a-keyboard-shortcut-doesnt-work-mchlp2864/mac) [keyboard shortcut](https://support.apple.com/en-us/HT201236) e.g. Control-Shift-F1.  
   - From Automator menu: Services -> Services Preferences (or, from System Preferences:  Keyboard -> Shortcuts -> Services)
   - Locate harp-Screenfix and add shortcut.
