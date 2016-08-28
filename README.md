# A postcard bot 

This bot can order a postcard for you.
A sample exchange goes like this:

Hello postbot

                            Never miss a birthday again by scheduling a birthday card.
                            Name a friend you'd like to send a postcard to.
                            Choose an upcoming birthday or type in a name.
                            |  Alex                 |
                            |  Gavin                |
                            |  Jess                 |

Jess
                            You've selected Jess. Please upload an image for your greetings card

(upload image)
                            Great, this is what it will look like.
                            ---------------------------------
                            |                               |
                            |         *          *          |
                            |                               |
                            |               I               |
                            |          ____________         |
                            |                               |
                            ---------------------------------

                            Please type in the address to post the card to
1 hacker way
                            is that 1 hacker way, menlo park, CA?
yes
                            Would you like to send it for 1st September, 2016?
yes
                            Great, press pay when you're ready. I'll provide a receipt.
                            ---------------------
                            |  Pay $1.50        |
                            ---------------------
Pay
                            ---------------------
                            | Receipt:          |
                            | Postcard $1.50    |
                            ---------------------

                            Would you like me to recur this postcard for next year?
No thanks
                            No problem. Would you like me to notify you?
Sounds great!

# Messenger Platform Sample -- node.js

This project is an example server for Messenger Platform built in Node.js. With this app, you can send it messages and it will echo them back to you. You can also see examples of the different types of Structured Messages. 

It contains the following functionality:

* Webhook (specifically for Messenger Platform events)
* Send API 
* Web Plugins
* Messenger Platform v1.1 features

Follow the [walk-through](https://developers.facebook.com/docs/messenger-platform/quickstart) to learn about this project in more detail.

## Setup

Set the values in `config/default.json` before running the sample. Descriptions of each parameter can be found in `app.js`. Alternatively, you can set the corresponding environment variables as defined in `app.js`.

Replace values for `APP_ID` and `PAGE_ID` in `public/index.html`.

## Run

You can start the server by running `npm start`. However, the webhook must be at a public URL that the Facebook servers can reach. Therefore, running the server locally on your machine will not work.

You can run this example on a cloud service provider like Heroku, Google Cloud Platform or AWS. Note that webhooks must have a valid SSL certificate, signed by a certificate authority. Read more about setting up SSL for a [Webhook](https://developers.facebook.com/docs/graph-api/webhooks#setup).

## Webhook

All webhook code is in `app.js`. It is routed to `/webhook`. This project handles callbacks for authentication, messages, delivery confirmation and postbacks. More details are available at the [reference docs](https://developers.facebook.com/docs/messenger-platform/webhook-reference).

## "Send to Messenger" and "Message Us" Plugin

An example of the "Send to Messenger" plugin and "Message Us" plugin are located at `index.html`. The "Send to Messenger" plugin can be used to trigger an authentication event. More details are available at the [reference docs](https://developers.facebook.com/docs/messenger-platform/plugin-reference).

## License

See the LICENSE file in the root directory of this source tree. Feel free to useand modify the code.
