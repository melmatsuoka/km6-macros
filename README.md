km6-macros
==========

A collection of Keyboard Maestro 6 macros that make my life worth living.


clipboard
=========

* Kindle Clipboard Cleaner: Strips out the annoying "annotation" that gets appended to all text that you select and copy in Kindle.app. I recommend mapping this to ⌘V, so as not to interrupt your normal copy/paste muscle memory.

Compressor
==========

* UC to ProResHQ: This is intended to be run from the Terminal/command-line. It will recursively search for all Uncompressed 8/10-bit 4:2:2 QuickTime movies in the the current working directory/folder, then uses the Compressor command-line interface to convert them to ProRes HQ files. The ProRes files are written to the same folder that the original uncompressed source file is locate.  Requires Compressor 4.1 or higher.

Premiere Pro CC
===============

* Goto 2-pop: Moves the timeline playhead to the 2-pop (assumes that your 2-pop starts at 00:59:58:00)

* Delete Empty Tracks: Deletes all empty video & audio tracks in the active timeline.

* Force Creative Cloud Settings Sync: A crazy macro that will auto-fill the "Adobe Creative Cloud Authentication" dialog with your Adobe ID & password. I built this out of frustration with the fact that the Creative Cloud Sync authentication seems to have no integration with the OS X System Keychain, so every time you restart Premiere, you have to enter your credentials all over again. Considering the fact that I use lengthy and randomized passwords which I don't even have memorized (I use the "1Password" password manager to store and recall all my passwords), having to manually open 1Password to copy and paste the password info gets old really fast. The macro pulls the login/password info from the OS X System Keychain, rather than having to hardcode the credentials into the KM Macro itself, so it's relatively secure. For maximum user-friendliness, it also allows the user to create the Keychain item for their Adobe ID, directly from the Macro itself (rather than having to do it manually in Keychain Access.app). This was a fun exercise in using some of the more obscure features of Keyboard Maestro, such as regex matching of dynamic menu titles, and simple User Input validation. 

* Increment Sequence: Emulates FCP7 sequence incrementing behavior. It will create a backup copy of the currently selected sequence in the Project panel, then numerically increments the active sequence name in place. In order for this Macro to work, the name of your initial sequence must *end* with a zero-padded number, for example: "sequence_name 01"



