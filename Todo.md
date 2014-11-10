## PORTFOLIO TODO

### Axis version (2 weeks)
- [x] Update implementation
- [ ] Update application files (not just Structure) (C# updater?)
- [ ] Log list (what was updated)
- [ ] Installer: With Axis corporate languages
- [ ] Fix Entry wrong offset when opening/closing

### Waiting for feedback, lower prio (1 week)
- [ ] Google Analytics (what should be tracked?)
- [ ] Theming of the application (to better support several versions)
- [ ] Mp4 movies in the Structure

### Misc (1 week)
- [ ] Editmode: fix playlist view scrolling direction: from vertical ==> horisontal
- [ ] Installer: Language/Tetra Pak versions
- [ ] Installer: pack as a self-extracting zip
- [ ] Subfolders in My Presentations

## Server updates
- [ ] Cache SHA1 hashes (so that update checks are faster and requires less processing)

## DONE
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

