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

