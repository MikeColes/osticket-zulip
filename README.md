osTicket-Zulip
==============
A plugin for [osTicket](https://osticket.com) which posts notifications to a [Zulip](https://zulipchat.com/) stream.

Forked from: [https://github.com/MikeColes/osticket-zulip](https://github.com/MikeColes/osticket-zulip) to update Zulip compatibility. Tested on Zulip 4.2

Forked from: [https://github.com/clonemeagain/osticket-slack](https://github.com/clonemeagain/osticket-slack)

Which was originally forked from: [https://github.com/thammanna/osticket-slack](https://github.com/thammanna/osticket-slack).

Info
------
This plugin uses CURL and tested on osTicket-1.15.2

## Requirements
- php_curl
- A Zulip bot account configured to be an incoming webhook. This project uses the "slack" webhook which is likely https://[your domain]/api/v1/external/slack

Install
--------

## Zulip Setup
- Login to Zulip
- Click the gear in the upp, right-hand corner, select 'Settings'
- Select 'Your Bots'
- Select 'Add a new bot'
- Select 'Incoming Webook', Give a name to your bot and record your settings to be added to the osTicket configuration.
- Click 'Create Bot'

## osTicket Install
Clone this repo or download the zip file and place the contents into your OSTicket install `uploads/include/plugins` folder.
Login to your Agent Panel > Manage > Plugins, enter your Zulip bot details from above

## Test!
Create a ticket!

You should see a message posted in your Zulip stream and channel you setup in the configuration

