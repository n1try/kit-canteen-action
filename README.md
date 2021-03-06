# kit-canteen-action

![](https://i.imgur.com/nS6amev.png)

This is the backend for a (currently unpublished), [Dialogflow](https://dialogflow.com)-based Google Home action to get the diet of [Mensa am Adenauerring](http://www.sw-ka.de/en/essen/) at the [Karlsruhe Institute of Technology](https://kit.edu). It supports English and German language, however, since the meals are only available in German, English pronounciation isn't too good. Data is fetched from [openmensa](https://openmensa.org). Thanks for that project!

## How to run?
* Import contents from [dialogflow_export](/blob/master/dialogflow_export) as a ZIP file into your Dialogflow project
* Install NodeJS on your server 
* Clone this repo
* Set environment variables for `PORT` and `DEBUG` or create `.env` file
* Run this script (`npm start`)
* Point the fulfilment webhook in Dialogflow to the URL at which your script is listening (_HTTPS_ required). Alternatively you can host this script using Cloud Functions or AWS Lambda.

## How to use?
Currently, the action is not publicly available. However, if you run it as your own actions linked to your Google account, it can be invoked as follows.
* _"Hey Google, ask **KIT Canteen** what to eat today"_
* _"Hey Google, talk to KIT Canteen"._ ..._"What's in the canteen on thursday?"_
* _"Hey Google, frag **KIT Mensa**, was es heute zu essen gibt"_
* _"Hey Google, sprich mit KIT Mensa"_ ... _"Was gibt es morgen zu essen?"_

## License
MIT @ [Ferdinand Mütsch](https://ferdinand-muetsch.de)
