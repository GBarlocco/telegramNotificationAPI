# How to send a notification with Telegram API :calling:

## Introduction
In this post I will explain how to send notifications using the Telegram API. This script can be applied to PLCs, databases, drivers, etc.

[![Telegram-logo.png](https://i.postimg.cc/3wq0vqVJ/Telegram-logo.png)](https://postimg.cc/SXWK0gmw)

## App
I will explain how to do all the configuration step by step

### Create the bot

* First you must create the bot, for this it is necessary to execute commands in BotFather [BotFather](https://telegram.me/BotFather)
> [![bot-Father.png](https://i.postimg.cc/Y0RdMkDC/bot-Father.png)](https://postimg.cc/XBZfgM0R)

* Then you must select /newbot  and follow the instructions, it is easy to do
>  [![botfather-commands.png](https://i.postimg.cc/rpv40bRC/botfather-commands.png)](https://postimg.cc/QBJCvfbH)

* At the end of the bot creation, you will need the token
> [![Token-bot.png](https://i.postimg.cc/fTLbsCJw/Token-bot.png)](https://postimg.cc/5jhJqwBG)

* We execute the /start command in the bot chat
> [![bot-start.png](https://i.postimg.cc/C1SFQH3p/bot-start.png)](https://postimg.cc/zL2ZLWDx)

* The next step is to create the group on Telegram and add it. Remember that the bot will send messages to the group
> [![add-bot.png](https://i.postimg.cc/xdqGbMxY/add-bot.png)](https://postimg.cc/06RKTM1H)

* To send notifications to the group you will need to know the ID. We add to the group "ChatID"
> [![chat-id.png](https://i.postimg.cc/59ptDT97/chat-id.png)](https://postimg.cc/7bGD2B20)

* Now it's time to program in Node-RED. First we must install node-red-contrib-telegrambot

* Then we will configure the bot, for this we must use the Token
> [![add-token.png](https://i.postimg.cc/LXbb1mBQ/add-token.png)](https://postimg.cc/yg0jq4G0)

* Now we program the function in charge of containing the message and the configuration
> [![function-message.png](https://i.postimg.cc/dt2czT9q/function-message.png)](https://postimg.cc/nChWmr55)
> [![debug-message.png](https://i.postimg.cc/hvR3rp6V/debug-message.png)](https://postimg.cc/62z06L9Q)

* Finally the program will look like this
> [![flow.png](https://i.postimg.cc/MKxFf3yS/flow.png)](https://postimg.cc/kD1ckc11)

*When enabling the function (information from the PLC, Driver, database), the message will be sent
> [![hello-world.png](https://i.postimg.cc/tC22Zqq3/hello-world.png)](https://postimg.cc/kBRxLdtG)


## Author
> <p>Gastón Barlocco. </p>
> <p>Email: barlocco@hotmail.es </p>


## Libraries

| Library                                                                       |                                                                      
| ----------------------------------------------------------------------------- |             
| [Telegram Bot](https://flows.nodered.org/node/node-red-contrib-telegrambot)   | 



## Installers

Telegram bot:
``` 
npm install node-red-contrib-telegrambot
```

## Scripts

#### `node-red`
Run the application locally
[http://127.0.0.1:1880/](http://127.0.0.1:1880/)



## Extra
* [Documentation](https://nodered.org) Node-RED
* [Documentation](https://nodejs.org/es/) Node Js