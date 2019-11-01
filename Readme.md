# Level One Challenge
[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/) [![ForTheBadge uses-js](http://ForTheBadge.com/images/badges/uses-js.svg)](http://ForTheBadge.com) [![ForTheBadge built-with-love](http://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/Naereen/) [![GitHub license](https://img.shields.io/github/license/Naereen/StrapDown.js.svg)](https://github.com/Naereen/StrapDown.js/blob/master/LICENSE)

**Front End** - - - - - - - **Back End**

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/53765614911d45bca78fab6d835d795d)](https://www.codacy.com/manual/jacob13400/FrontEnd?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=YE-Stack/FrontEnd&amp;utm_campaign=Badge_Grade)   [![Codacy Badge](https://api.codacy.com/project/badge/Grade/aea362f304c449e986e288c7c5c2ef85)](https://www.codacy.com/manual/jacob13400/Notify?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=YE-Stack/Notify&amp;utm_campaign=Badge_Grade)
## Description
This is a project which was built to achieve the following requirements.

1.Take a few inputs through android application. Numbers and Text.

2.Store it in a non local database.

3.Access the data (stored in database on web ) through a web app.

4.Take some other inputs through web app. Numbers and Text.

5.Process both these inputs and create an output.

6.Send result from Web app to android app on submission of output to Android app and display it on app through a notification.

7.Notify Web app user & Android app user through whatsapp and SMS

## Our Implementation
**The App** - -> The app accepts a string and a text from the user and then sends it to the database. This triggers a Whatsapp and SMS notification to be sent to the web user.

**The WebSite** - -> The web user enters a string and number on the website which is then sent to the backend. Here the two strings are concatinated, the two numbers added and the result is sent back to be displayed on the website. Whatsapp and SMS notifications are sent to the app user and the final output is displayed in the app too. The app user also gets a push notification when the output is prepared.
### Tech Stack 
* The mobile app has been built using React Native - -[ReactNative](https://facebook.github.io/react-native/)
* The web app using Bootstrap - -[Bootstrap](https://getbootstrap.com/)
* Firebase acts as non-local realtime database and also facilitates push notifications - -[Firebase](https://firebase.google.com/)
*  The Twilio API has been used as the gateway for sending Whatsapp and SMS notifications to the web and mobile user. - -[Twilio](https://www.twilio.com/)
* Django handles the working of the website and the backend of the implementation. - -[Django](https://djangogirls.org/)

**The twilio and Firebase integrations we have used are free trial implementations but when scaling paid plans would have to be used.**

![Twilio](data:image/png;base64,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)![Firebase](https://miro.medium.com/max/2560/1*RdowFHAWDgkkwjXkQW0yNQ.png )
## Getting Started

### Version Information
[![Generic badge](https://img.shields.io/badge/<Firebase>-7.2.2-red.svg)](https://shields.io/)   [![Generic badge](https://img.shields.io/badge/<ReactNative>-0.61.3-blue.svg)](https://shields.io/) [![Generic badge](https://img.shields.io/badge/<React>-16.9.0-teal.svg)](https://shields.io/)  [![Generic badge](https://img.shields.io/badge/<Django>-2.2.6-<COLOR>.svg)](https://shields.io/)  

### Getting You Set Up
Our implementation works consdering you have set up the following prerequisites ->
*  **Your device has Python 3** 
* **Django is installed**
* **React native is setup on your device**
* **The numbers being used for Whatsapp and SMS services are authenticated with Twilio so please make sure your numbers are registered**



### Installing
Inside Front-End Folder
```
npm install
```
```
react-native run-android
```
```
react-native start
```
Inside Notify folder
```
pip install -r requirements.txt
```
To start the server
```
./manage.py runserver
```
## Screenshots
![screen1](https://github.com/YE-Stack/YEStack1/raw/master/docs/assets/images/appinput.jpg )

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

