const Discord = require('discord.js');

const client = new Discord.Client();

 

client.on('ready', () => {

    console.log('I am ready!');

});

 

client.on('message', message => {

    if (message.content === 'ping') {

       message.reply('pong');

       }

});

 

// THIS  MUST  BE  THIS  WAY

client.login(process.env.BOT_TOKEN);//where BOT_TOKEN is the token of our bot
{

  "name": "IPL Bot",

  "description": "For IPL",

  "version": "0.0.0",

  "main": "bot.js",

  "scripts": {

    "start": "node bot.js"

  },

  "dependencies": {

    "discord.js": "11.1.0",

    "request": "2.81.0"

  }

}
worker: node bot.js
