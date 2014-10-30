## TODO

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
- [ ] Process UpdateBundle (Check if Package.json exists and then...)
    - [x] Delete: Files
    - [x] Delete: Folders
    - [x] Create: Folders
    - [x] Move: Downloaded Files
    - [ ] Dispatch Complete event

### Update workflow
- [ ] Startup (precheck only)
- [ ] Check for update Package
    - [ ] Yes: Install update package
    - [ ] No: Goto next step...
- [ ] Start "Main" app
- [ ] Compare
    - [ ] Has changes:
        - [ ] Prompt user, if yes, cont.
        - [ ] Download
        - [ ] On download complete, prompt for restart, if yes, cont.
        - [ ] Restart
    - [ ] End Update check

