# EduHive App

EduHive is a product of Tech Hive Limited, which is the first e-learning platform in Bangladesh where students from class 9 to 12, University Admission Examinees, BCS & Other Jobs Entrance Examinees can take courses or prepare for exams from their preferred teachers or coaching centres.

Model Tests for admission tests for Dhaka University (DU), Jahangirnagar University (JU), Khulna University (KU), Rajshahi University (RU), Chittagong University (CU), BUP, Agricultural University, SUST, BUET, RUET, KUET, CUET, other public and private universities of Bangladesh offered by Retina, UCC, OMECA, uniaid, Icon Plus, Icon, Primate, Climax, Prantik, Confirm, Physics Care, Biology Care, Math Lab, Chemistry Zone and other popular coaching centers of Banglaadesh.

EduHive is an easy learning app for the students of Bangladesh. Students from any group, science, arts (humanities), commerce (business studies) can learn any complex subject like Mathematics, Physics, Chemistry, Biology, Accounting, Management, Finance, English, Bangla and any other academic and admission courses through EduHive.

BCS, Bank Jobs, Teacher registration and any other Job seekers can also prepare themselves by taking model tests in EduHive.


### Clone & install

In the root directory
* Clone this repo `git clone https://github.com/techhivebd/eduhive-mobile-app.git`
* Install dependencies: `npm install` || `yarn install`


### iOS

In the `ios` directory

* Install Pods: `gem install cocoapods`
* Install Pods: `pod install`
* Install xcpretty: `gem install xcpretty`
* Launch: `open Sample.xcworkspace`
* To run from command line try: `react-native run-ios` || `yarn ios`


### Android

* You might need to do this to run it in Android Studio or on real device: `adb reverse tcp:8081 tcp:8081`
* And for the sample server: `adb reverse tcp:3000 tcp:3000`
* To run from command line try: `react-native run-android` || `yarn android`

### Building an APK

To build a signed APK

1. Close all other development resources for the project.
2. Run npm run build:android to first build the project.
3. In Android Studio, choose Build > Generate Signed APK.
4. Build a release APK by following the instructions in the GUI

To build a debug APK
* `$ react-native bundle --dev false --platform android --entry-file index.android.js --bundle-output ./android/app/build/intermediates/assets/debug/index.android.bundle --assets-dest ./android/app/build/intermediates/res/merged/debug`
* `$ cd android && ./gradlew assembleDebug`


### Server

There is a server that the app hits for data. The data is only stored in memory, but it should produce a more realistic environment.

In the `eduhive` web project

* Install dependencies: `yarn install`
* Run it: `yarn dev-server`

# Current Concepts

### Navigation

What follows within the Fundamentals section of this documentation is a tour of the most important aspects of React Navigation. It should cover enough for you to know how to build your typical small mobile application, and give you the background that you need to dive deeper into the more advanced parts of React Navigation.

#### Redux

The Components use Actions. Actions tend to use the API Services and dispatch an event. The Stores are listening to the events. The Components add and remove listeners to the Stores.

#### Data storage

Info is currently stored as json to the local file system.

#### API

It uses superagent to do HTTP requests and sets headers and other things like that.

#### Components

Some shared components that might be helpful

* SegmentedControl: Non-iOS specific version of that control
* SimpleList: make a list out of the props set
* Button: Helper to make them all similiar

### Things to test and improve

* Remove unused code
* Need to refactor old code
* Make habit to new react, react native and hooks 
* Maintain arbnb guidline and best practices
* Commenting and documentations


### Need to fix
- [ ] New alert(DropsownAlert) instead of React native Alert
- [ ] Tutors home scrollable
- [ ] Exam mcq item line break


## License

EduHive 2021
