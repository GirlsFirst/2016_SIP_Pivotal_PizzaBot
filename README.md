## Synopsis

Pizza Bot is an app on Facebook Messenger that enables a user to order a customized pizza with a click of a few buttons. The app is currently not linked to a pizzeria's API, so the current model will not follow through with ordering a pizza.

## License
Pizza Bot is protected by the Apache License, Version 2.0. This license allows the public to modify a copy of the software as long as the required notices are included. See this link for more information: http://www.apache.org/licenses/LICENSE-2.0 .

## Code Example

function inputAddress(payload, recipientId) {
    var deliverTo = payload.deliverTo;
    var user = payload.user;
    var message = {
       "attachment": {
           "type": "template",
           "payload": {
               "template_type": "generic",
               "elements": [{
                   "title": "Please Enter Your Address:",
                   "subtitle": "Street, City, State, Zip Code"
               }]
           }
       }
   };
   getDeliveryAddress = "true";

   return message;
};

## Motivation

The Pizza Bot was conceived to mitigate the frustrations of ordering a pizza over the phone or on a complicated website. Bots have the potential to become technology present in our everyday lives because of their accesibility and simple nature. Facebook Messenger is a popular platform among the Pizza Bot's target audience, making this bot very practical.

## Installation

Because Pizza Bot is not accesible to the public at the moment, to test the bot please like and message the following Facebook page: https://www.facebook.com/Pizza-Bot-1072653646143557/?fref=ts. An administrator will make you a test user shortly after your request.

## API Reference

Because the Pizza Bot is not linked to a pizzeria yet, there are no APIs in the code. However, the bot requires the use of a personal app made on Heroku.

## Contributors

In order to modify this bot, you must make your own Heroku app linked to a Facebook page. To get started, check out this tutorial: http://x-team.com/2016/04/how-to-get-started-with-facebook-messenger-bots/. After you have successfully created a bot, you may take the Pizza Bot's code and copy it into your index.js file.
 X-Team
How To Get Started With Facebook Messenger Bots | X-Team
This tutorial will show you how to setup and deploy simple Facebook Messenger Bot, using the Messenger Send/Receive API. (113KB)
April 25th at 10:33 AM
