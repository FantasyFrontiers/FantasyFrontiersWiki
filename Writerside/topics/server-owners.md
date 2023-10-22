# The Server Owner's Guide

### Introduction

This guide will teach you how to set up Fantasy Frontiers on your server, and how to configure it to your liking.


### Installation

##### Requirements

You will need the following to set up Fantasy Frontiers on your server:

- At least one dedicated text channel for the bot to use.


##### Adding the Bot to Your Server

Invite this bot to your server. You can do so by clicking [here](https://discord.com/api/oauth2/authorize?client_id=609710444021809152&permissions=0&scope=bot%20applications.commands).
- For security reasons, we will not include any global permissions in the bot. You will have to manually grant the bot the permissions it needs to function on your server.



### Configuration

##### Setting Up the Bot

Choose a channel for the bot to use. This channel will be used as main hub for the users to interact with.

In this channel, the bot needs the following permissions:

```
- Send Messages
- Send Embeded Links
- Send Files
```


- Once you have invited the bot to your server, you will need to set up the bot. You can do so by running the `setup panels` command in the channel.
- The bot will ask your preferred language. You can currently choose between English and German. (If you want to help us translate the bot, please refer to the [Contribution Guidelines](contribution-guidelines.md))


##### Advanced Configuration

If you want to configure the bot further, you can do so by running the `setup advanced` command in the channel. This will open a configuration panel, where you can change the following settings:

- System Announcements
  - Enable or disable system announcements and choose the channel/thread to send them to.
- Role Management
  - Setup special roles that will be automatically assigned to users when they join an ingame guild.