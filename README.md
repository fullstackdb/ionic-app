# Cordova Ionic Starter

The Cordova Ionic Starter with i18n support.
### Dependencies

Before you start develop, make sure that you have installed following stuff

| Dependency name  | Command to check       | Command to install                     | Documentation                    |
| ---------------- |:----------------------:| --------------------------------------:| --------------------------------------:|
| nodejs           | node -v                | [download](https://nodejs.org/en/)      | [node](https://nodejs.org/en/)      |
| npm              | npm -v                 | npm install npm@latest -g               | [npm](https://www.npmjs.com/)
| cordova          | cordova -v             | npm install -g cordova                  | [cordova](http://cordova.apache.org/docs/en/latest/) |
| ionic            | ionic -v               | npm install -g ionic cordova            | [ionic](https://nodejs.org/en/)


### Run app

After instalation dependencies, run following command in your command line:

```
ionic start myApp super
``` 

where myApp - name of your app.

In command line you will see instruction for next steps.

After generating app, you will able to use next commands:


| Command                                | Description            | 
| -------------------------------------- |:-----------------------------------:| 
| `ionic serve`                          | For run your app in browser         | 
| `ionic cordova run <platform name>`    | For run your app on device          | 
| `ionic build`                          | For build your app in static files  |
| `ionic cordova build <platform name>`  | For build your app for specific OS  | 


### Structure

```
| src
-| app
---| app.component.ts
---| app.module.ts
---| app.scss
---| main.ts
-| assets
---| i18n
---| icon
---| img
-| mocks
-| models
-| pages
-| providers
-| theme
-| index.html
-| manifest.json
-| service-worker.js
```

### Advices

Async code

```
constructor(private zone: NgZone, private service: ExampleService) {}

this.service.getData().subscribe((data: Data) => {
  zone.run(() => {
    // your async code
  })
})
```

'Routing'

```
constructor(private nav: NavController) {}

this.navCtrl.push(ItemDetailPage, {
    item: item
});
```