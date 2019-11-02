# Level One Challenge
[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/) [![ForTheBadge uses-js](http://ForTheBadge.com/images/badges/uses-js.svg)](http://ForTheBadge.com) [![ForTheBadge built-with-love](http://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/Naereen/) [![GitHub license](https://img.shields.io/github/license/Naereen/StrapDown.js.svg)](https://github.com/Naereen/StrapDown.js/blob/master/LICENSE)

**Front End** - - - - - - **Back End**

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/53765614911d45bca78fab6d835d795d)](https://www.codacy.com/manual/jacob13400/FrontEnd?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=YE-Stack/FrontEnd&amp;utm_campaign=Badge_Grade)   [![Codacy Badge](https://api.codacy.com/project/badge/Grade/aea362f304c449e986e288c7c5c2ef85)](https://www.codacy.com/manual/jacob13400/Notify?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=YE-Stack/Notify&amp;utm_campaign=Badge_Grade)
## Description
This is a project which was built to achieve the following requirements.

1.Take a few inputs through android application. Numbers and Text.

2.Store it in a non local database.

3.Access the data (stored in database on web ) through a web app.

4.Take some other inputs through web app. Numbers and Text.

5.Process both these inputs and create an output.

6.Send result from Web app to android app on submission of output to Android app and display it on app through a notification.

7.Notify Web app user & Android app user through Whatsapp and SMS. A push notification is sent to the app user too. 

## Our Implementation
**The App** - -> The app accepts a string and a text from the user and then sends it to the database. This triggers a Whatsapp and SMS notification to be sent to the web user.

**The WebSite** - -> The web user enters a string and number on the website which is then sent to the backend. Here the two st are rings are concatenated, the two numbers added and the result is sent back to be displayed on the website. Whatsapp and SMS notifications are sent to the app user and the final output is displayed in the app too. The app user also gets a push notification when the output is prepared.
### Tech Stack 
* The mobile app has been built using React Native Expo - -[Expo](https://docs.expo.io/versions/latest/)
* The web app using Bootstrap - -[Bootstrap](https://getbootstrap.com/)
* Firebase acts as non-local realtime database and also facilitates push notifications - -[Firebase](https://firebase.google.com/)
*  The Twilio API has been used as the gateway for sending Whatsapp and SMS notifications to the web and mobile user. - -[Twilio](https://www.twilio.com/)
* Django handles the working of the website and the backend of the implementation. - -[Django](https://djangogirls.org/)

**The twilio and Firebase integrations we have used are free trial implementations but when scaling paid plans would have to be used.**

![Twilio](https://www.vectorlogo.zone/logos/twilio/twilio-ar21.svg)![Firebase](https://www.vectorlogo.zone/logos/firebase/firebase-ar21.svg )
## Getting Started

### Version Information
[![Generic badge](https://img.shields.io/badge/<Firebase>-7.2.2-red.svg)](https://shields.io/)   [![Generic badge](https://img.shields.io/badge/<Expo>-3.2.3-blue.svg)](https://shields.io/) [![Generic badge](https://img.shields.io/badge/<React>-16.9.0-teal.svg)](https://shields.io/)  [![Generic badge](https://img.shields.io/badge/<Django>-2.2.6-<COLOR>.svg)](https://shields.io/)  

### Getting You Set Up
Our implementation works considering you have set up the following prerequisites ->
*  **Your device has Python 3** 
* **Django is installed**
* **React native is setup on your device**
* **The numbers being used for Whatsapp and SMS services are authenticated with Twilio so please make sure your numbers are registered**

### Credentials Information
**Please make sure that you add all the necessary authentication data pertaining to Firebase and Twilio to [credentials_sample.py](https://github.com/YE-Stack/Notify/blob/master/credentials_sample.py) before installing and running. Rename it to "credentials.py"**

### Installing

#### Setting up the mobile app:

* Go to the parent folder of the app and run the following code. This installs all the dependencies required by the app.
```
npm install
```
* This starts a expo development server for the app and gives you a url to it.
```
expo start
```
* To run the app on an android, you need to add your device to **adb devices** list. Follow this [guide](https://facebook.github.io/react-native/docs/running-on-device).

* Make sure that your android device and the expo server are connected to the same network.

* After the terminal shows "Successfully ran adb reverse". Either scan the QR code (this requires **Expo** app, which can be installed from [here](https://play.google.com/store/apps/details?id=host.exp.exponent&hl=en_IN)) or just press 'a', this automatically installs the debug app and runs it.

##### If you want to directly install the app, click [here](https://exp-shell-app-assets.s3.us-west-1.amazonaws.com/android/@narddoggo/new-02b8286b17364c86a805b76c51af4b45-signed.apk) for the .apk file. 

Or scan this using [Expo](https://play.google.com/store/apps/details?id=host.exp.exponent&hl=en_IN) app.

![qr code](docs/assets/images/qr.png)


#### Setting up the Django backend server:

* Go to the parent folder of the Django server and run the following code. This installs all the required dependencies. 
```
pip install -r requirements.txt
```
* Start the server and click on the url to access the web app.
```
./manage.py runserver
```
## Screenshots
![screen1](https://github.com/YE-Stack/YEStack1/raw/master/docs/assets/images/appinput.jpg)

![screen3](https://github.com/YE-Stack/YEStack1/raw/master/docs/assets/images/output.png)

![screen3](https://github.com/YE-Stack/YEStack1/raw/master/docs/assets/images/output2.png)

![screen4](https://github.com/YE-Stack/YEStack1/raw/master/docs/assets/images/appoutput.jpg )

![screen5](https://github.com/YE-Stack/YEStack1/raw/master/docs/assets/images/message.jpg)

![screen6](https://github.com/YE-Stack/YEStack1/raw/master/docs/assets/images/whatsapp.jpg )

## Authors


<table>
  <tr>
    <td align="center"><a href="https://github.com/jacob13400"><img src="https://avatars2.githubusercontent.com/u/45292374?s=400&v=4" width="80px;" alt="Ricky Robinett"/><br /><sub><b>Jacob Abraham</b></sub></a><br /><a title="Code">
    <td align="center"><a href="https://github.com/ebby21"><img src="https://avatars3.githubusercontent.com/u/44583376?s=400&v=4" width="80px;" alt="Ricky Robinett"/><br /><sub><b>Abraham Francis</b></sub></a><br /><a title="Code">
    <td align="center"><a href="https://github.com/bat-fleck"><img src="https://avatars2.githubusercontent.com/u/47271375?s=460&v=4" width="80px;" alt="Vishnu Prakash"/><br /><sub><b>Vishnu Prakash</b></sub></a><br /></td>
    <td align="center"><a href="https://github.com/krishnapsn"> <img src="https://avatars0.githubusercontent.com/u/44611063?s=400&v=4" width="80px;" alt="Teddy Gustiaux"/><br /><sub><b>Krishna Prasad</b></sub></a><br /></td>
    <td align="center"><a href="https://github.com/SriniPai285"><img src="https://avatars0.githubusercontent.com/u/48677009?s=460&v=4" width="80px;" alt="Aidan Smith"/><br /><sub><b>Srinivas R Pai</b></sub></a><br /></td>
  </tr>
</table>

## License

This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/YE-Stack/YEStack1/blob/master/License.md) file for details

## Acknowledgments

We would like to acknowledge everyone involved in the project for all the work that they put in. 

P.S 
Anyone intrested in contributing can go ahead and submit a pull request.

[![Ask Me Anything !](https://img.shields.io/badge/Ask%20Us-anything-1abc9c.svg)](https://github.com/jacob13400)

