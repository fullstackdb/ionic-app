# Test app

### Dependencies

Before you start develop, make sure that you have installed following stuff

| Dependency name  | Command to check     | Command to install                     | Documentation                    |
| ---------------- |:--------------------:| --------------------------------------:| --------------------------------------:|
| nodejs           | node -v              |(download)[https://nodejs.org/en/]      | (node)[https://nodejs.org/en/]      |
| npm              | npm -v               |npm install npm@latest -g               | (npm)[https://www.npmjs.com/]
| cordova          | cordova -v           |npm install -g cordova                  | (cordova)[http://cordova.apache.org/docs/en/latest/] |
| ionic            | ionic -v             |npm install -g ionic cordova            | (ionic)[http://ionicframework.com/docs/] |


### Run app

After instalation dependencies, run following command in your command line:

```
ionic start mySuperApp super
``` 

where mySuperApp - name of your app

In command line you will see instruction for next steps.

After generating app, you will able to use next commands

`ionic serve` For run your app in browser

`ionic cordova run ios` `ionic cordova run android`  For run your app on device

`ionic build` For build your app in static files.

`ionic cordova run build ios` `ionic cordova run build android` For build your app for specific OS