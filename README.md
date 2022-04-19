# AutoCAT

Automated Computer-Aided Testing

A simple but powerful interface running test scripts.

Features:
- Tests/Standards/Specs/Playlists
- A queue
- Pause, play, skip, loop
- Tree style layout (allows user to change multiple scripts by changing the parent branch)
- Support for drag and drop style editing
- Export data directly into reports
- An additional gui for selecting test scripts (easier to use than tree view but does not allow editing branches)

Needs to support:
- Saving and managing variables for test scripts to use
- Passing variables from one test script to another (Storing variables in a place where the script can access them.)
- Scripts that communicate over TCP/IP (Maybe it needs a sister program if it gets too bloated)
- Python, CMD, Powershell, and any peripheral device switching or save states which those scripts create. 
  (example: a script that saves data to a json file for later use)
- a force shutdown (hotkey and pushbutton)
- Automatic file naming and directory creation
- Editing existing reports aswell as creating new ones

Does NOT need to support:
- a method for creating test scripts
- a method for managing files created by those test scripts
- trash collection should be handled by the test script
-> Everything that the user wants to do is allowed, the tests are performed by the test scripts not AutoCAT. 
    AutoCAT is a gui for storing and running test scripts, not for doing the actual tests themselves.

May add support for:
- a global progress bar
- skip on error, create a separate queue of skipped tests to rerun
- **Add the ability to record A/V of tests for later review. Add timestamps for errors/failures.**
- OTA updates and installation manager
- Save window settings on close
- Support for long-term tests (sister program?)
  - Send email/other notification when test stops running (barometer logger)
  - lightweight
  - can run in the background in system tray or on headless devices
  - Ideally a script that was written and saved to the main computer can be run on the DUT computer without getting a flash drive and moving it manually.
    (also fix the obvious security risks of letting users run scripts on other computers over tcp)
  
Future additions?:
- Shuffle
- Advanced docking system
