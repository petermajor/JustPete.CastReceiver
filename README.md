# JustPete.CastReceiver

## Intro

The first steps in creating a custom cast receiver.

* Create a basic cast receiver that can receive messages
* Create a basic page for Chrome browser that can send messages

If this works you know that your Chromecast has been successfully registered as a developement device and that the Chromecast can connect to your computer that hosts the receiver.

## Steps to run

* [Register your Chromecast](https://developers.google.com/cast/docs/registration#RegisterDevice) as a developer device
* [Register new application](https://developers.google.com/cast/docs/registration) to get an _app id_. The url will be _http://<your-computer-ip>:9999/receiver.html_
* Clone the repo, set the current branch to _Step 1_ 
* Install express by running `npm install` in the repo root folder
* Put your _app id_ in the __applicationID__ variable in __demo.html__
* Start express by running `node app.js`
* Navigate to _http://<your-computer-ip>:9999/demo.html_ in your chrome browser.
* Click the Chromecast button on the top right of Chrome and select the device you registered earlier.
* The screen on the Chromecast TV should go black and have some text as the receiver is loaded
* Type a message into the input of your Chrome window and hit ENTER
* You should see that text on the Chromecast TV!

Thanks to the following site for demo.html code:
https://github.com/googlecast/CastHelloText-chrome

Thanks to the following site for receiver.html code:
http://blog.lemberg.co.uk/developing-chromecast-ready-application-android-platform