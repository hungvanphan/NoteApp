# Environment test
    Tested on Macos environment
    Tested device iOS
# Projects
    BackEnd_NoteApp project backend
    Mobile_FrontEnd_NoteApp project mobile frontend
# Command clear when mobile can not run

    Clear watchman watches: watchman watch-del-all
    Delete node_modules: rm -rf node_modules and run yarn install
    Reset Metro's cache: yarn start --reset-cache
    Remove the cache: rm -rf /tmp/metro-\*
    
    echo 256 | sudo tee -a /proc/sys/fs/inotify/max_user_instances
    echo 32768 | sudo tee -a /proc/sys/fs/inotify/max_queued_events
    echo 65536 | sudo tee -a /proc/sys/fs/inotify/max_user_watches
    watchman shutdown-server
# Dependencies
    brew install yarn
    brew install npm
    brew install node
    brew install watchman
    sudo gem install cocoapods
# Running your React Native application
    1. git clone https://github.com/hungvanphan/NoteApp.git
    2. cd BackEnd_NoteApp
    3. npm install
    4. node server.js
    5. cd Mobile_FrontEnd_NoteApp
    6. npm install
    7. cd ios/
    8. pod install
    9. npx react-native start
    10. npx react-native run-ios (if error go step 11)
    11. open xcode and run app
