This repo demonstrates crash while using react-native-navigation v7.24.3 and react-native-codepush. 

To reproduce crash:
- Create new application at microsoft appcenter + generate deployment keys https://appcenter.ms/
- Add "staging" deployment key at App.js:68
- Install production build of this app to device/simulator
- Change something in text to check that codepush update work (for example add some word to text at App.js)
- Create new codepush update with appcenter cli
- Restart application, crash

