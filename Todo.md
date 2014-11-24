## PORTFOLIO TODO
- [ ] Theming of the application (to better support several versions)
- [ ] Editmode: fix playlist view scrolling direction: from vertical ==> horisontal
- [ ] Mp4 movies in the Structure
- [ ] PDF Files in the structure
- [ ] Cache SHA1 hashes (so that update checks are faster and requires less processing)
- [ ] Log list (what was updated)
- [ ] Fix Entry wrong offset when opening/closing
- [ ] Installer: Language/Tetra Pak versions
- [ ] Google Analytics (what should be tracked?)
- [ ] Subfolders in My Presentations
- [ ] ~~Installer: With Axis corporate languages~~

## BUG TO FIX

## DONE
- [x] On restart if update is downloaded it will always install, and restart. Fix so that restart is only if the restart button is clicked!!
- [x] Update implementation
- [x] Update application files (not just Structure) (C# updater!)
- [x] Fix text margins
- [x] New icons
- [x] Fix logo
- [x] Update the structure to the current update version
- [x] Installer
- [x] Add ignore pattern option to SHA1_Folders (unins000.dat, unins000.exe)

### Update
- [x] Json encoding
- [x] Same format as the listings
- [x] Separate into actions
- [x] ListingCompare: Use param values from setting.json
- [x] DownloadQueue
    - [x] ProgressEvents - progress / total?
    - [x] VisualDownloadQueue
- [x] Process Comparison:
    - [x] Download files to local temp folder (Package)
    - [x] Save Comparison as Package.json file
    - [x] Dispatch event Complete
- [x] Process UpdateBundle (Check if Package.json exists and then...)
    - [x] Delete: Files
    - [x] Delete: Folders
    - [x] Create: Folders
    - [x] Move: Downloaded Files

### Update workflow
- [x] Startup (precheck only)
- [x] Check for Update Package
- [x] If Update Package = install
- [x] Start "Main" app
- [x] Compare
    - [x] Has changes:
        - [x] Prompt user, if yes, cont.
        - [x] Download
        - [x] On download complete, prompt for restart, if yes, cont.
        - [x] Restart
    - [x] End Update check

