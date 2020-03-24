# ViviHealth Patient App

### Before you start

ViviHealth requires a couple of previous steps to start with the installation. 

- You will need to have [npm](https://www.npmjs.com/) to install the application dependencies. If you don't have it, please follow [this](https://www.npmjs.com/get-npm)  steps to install it.
- You will need to belong to the apple organization development team for this project in order to run the application on iOS. 
- You will need access to a [this](https://github.com/transistorsoft/react-native-background-geolocation-android) private github repository to install this dependency:
```sh
react-native-background-geolocation-android
```
- Also, this is a React Native project, so you must install React Native. Follow [this](https://facebook.github.io/react-native/docs/getting-started.html#content) steps to do it.

### Installation

1. Clone the repo locally:

```sh
git clone git@github.com:recovery-ally/patient-app.git
```

2. Navigate into project
```sh
cd patient-app
```

3. Install dependencies
```sh
npm install
```

4. Configurate iOS project
```sh
cd ios
pod install
```

5. Go back to main project folder
```sh
cd ..
```

### Run application
You will need to run this application on a fisical device. This project is unable to run on emulator because of BioStrap dependency (library not built for Arm)
##### iOS ###
1. Open application in xcode
```sh
cd ios
open patientApp.xcworkspace
```

2. Configure signing on project target
-  Tap on patientApp project
- Tap Signing & Capabilities tab
- Tap on patientApp target
- On Team field, choose the development team from your apple account

3. Run the application: Product -> Run or just the play button

##### Android ###

1. Connect the device to your computer
2. Run application
```sh
npm run android
```
