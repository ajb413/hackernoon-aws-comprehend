# PubNub ChatEngine Demo with Amazon Comprehend

## Instructions
* Sign up for PubNub
* Sign up for Amazon AWS
* Run [ChatEngine Setup](https://www.pubnub.com/docs/chat-engine/getting-started#automagic-pubnub-setup)
* Get AWS `access` and `secret` keys for Comprehend guide [here](https://docs.aws.amazon.com/comprehend/latest/dg/auth-and-access-control.html)
* Go to the PubNub Functions event handlers in the [admin portal](https://admin.pubnub.com/)
* Add an `On Request` event handler (+ tab) and paste `comprehend-pfunc.js` contents into the editor
* To the left of the editor, click `MY SECRETS` and add `AWS_access_key` and `AWS_access_key`
* Click `COPY URL` and paste it in `app.js` as `comprehendFunctionURI` variable
* Copy the `Publish` and `Subscribe` keys for the app from the admin portal
* Paste them at the top of `app.js`
* Install https://www.npmjs.com/package/http-server or something similar and boot a new server from the root folder of this project
* `http-server`

## Features

There is a colored bubble based on the message sentiment analysis. Green for positive, grey for neutral, red for negative.

Uncomment under the `UNCOMMENT` lines in `app.js` to see ChatEngine features like 
* Chat History
* Typing Indicator Plugin 
* Markdown Plugin

![App Screenshot](https://github.com/ajb413/hackernoon-aws-comprehend/raw/master/screenshot.png "ChatEngine Demo")