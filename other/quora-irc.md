# Quora's IRC Guide

Hello all, I thought it would be a good idea to explain how to properly get on 
IRC using the best possible tools and how to set up things like NickServ 
accounts. All this information is targeted for the `irc.tulpa.info` servers, 
but with some research can be applied to almost any IRC network out there.

### Webchat

There are a few choices available for webchat these days. You can use:

 - [Mibbit](http://widget00.mibbit.com/?server=irc.tulpa.info&channel=%23tulpa)
 - [KiwiIRC](https://kiwiirc.com/client/irc.tulpa.info/?nick=tulpamancer|?#tulpa)
 - [LightIRC](http://irc.tulpa.info)

### Desktop Clients

Clients for a normal desktop computer can be somewhat weird. For best results 
I recommend using either of the following:

 - [ChatZilla](http://chatzilla.hacksrus.com/)
 - [HexChat](http://hexchat.github.io)

If you are not technically savvy, ChatZilla will likely be the easiest choice 
as it takes the least amount of setup (it is a Firefox plugin).

In most cases, initially connecting should be as easy as typing in:

`/server irc.tulpa.info`

From here you should pick a nickname using `/nick`.

`/nick YourNewNickHere`

### Registration with `NickServ`

Upon connecting, you will see a notice that looks like this:

`-NickServ(NickServ@services.tulpa.info)- Welcome to Tulpa.info, Quora2! Here on Tulpa.info, we provide services to enable the registration of nicknames and channels! For details, type /msg NickServ help and /msg ChanServ help.`

To register your nickname with services, you use the `NickServ` `REGISTER` 
command. The `REGISTER` command takes in your desired password and an email 
address. At this time email verification is **NOT** required, but the password 
reset process involves sending an email to one of the staff from the address on 
your `NickServ` account. Staff will **never** see your password.

An example is shown below:

`/msg NickServ register myPassword quora@domain.tld`

From now on, you will need to `IDENTIFY` to your chosen nickname by using:

`/msg NickServ IDENTIFY YourPassword`

or:

`/msg NickServ IDENTIFY YourAccountName YourPassword`

### Automatic Identifying

## Chatzilla

In the preferences window, select your server name (it should be 
`irc.tulpa.info`) and click on the "Lists" tab. Under the Auto-perform list, 
add `/ns id YourAccount YourPassword`. Mine looks
[like this](http://i.imgur.com/W5AdcEe.png)

## HexChat

Create a server profile for `irc.tulpa.info` if you haven't already. Mine looks 
[like this](http://i.imgur.com/byJhgON.png). Next, open the
[edit dialog](http://i.imgur.com/Z6pqHvU.png) and choose
[NickServ authentication](http://i.imgur.com/5wujiBv.png).

### Autojoining Channels

## Chatzilla

Right click on a channel tab and choose "Open This Channel at Startup". It will 
automatically open on startup.

## HexChat

The autojoin box in HexChat is in the edit dialog. Mine looks
[like this](http://i.imgur.com/PpZTFdL.png).

### Channels

Here are a few channels you might find interesting:

 - `#tulpa` - The network lobby and current biggest channel
 - `#redditulpas` - The channel for /r/tulpas
 - `#topic.info` - The on-topic discussion channel for http://tulpa.info forum members

To find more channels, use `/list` or `/msg ALIS LIST *`. `ALIS` is a service that does listing of channels by name, topic, usercount and a few other factors. See `/msg ALIS HELP` for details.

---

I hope this clears up some problems that people have had with the IRC channels. 
If you have any further questions, please ask in `#help` on `irc.tulpa.info` or comment on this thread. My reddit username is /u/Heartmender- and I will reply to any PM's as soon as possible.

~Quora

---

EDIT:

For those using Trillian's IRC feature, /u/technoManipulator made a sequence of screenshots outlining some of the settings.

First make an IRC account using "[Add Account](http://imgur.com/nZLQ1Gh,qxHpkxy,Yp2Pfr6#2)" from the Accounts section.

Under the account, put settings like [these](http://imgur.com/nZLQ1Gh,qxHpkxy,Yp2Pfr6#2). The Username can be whatever you want, as well as the nickname. People will see you by your chosen nickname, so be careful what you put there. The only necessary field is the Server. That has to be there.

Next, go to your Settings within the IRC account. Under "[Miscellaneous](http://imgur.com/nZLQ1Gh,qxHpkxy,Yp2Pfr6#0)" you should put in the command "/join #[Channel]" Where the brackets indicate a variable. The Channel variable can be `#tulpa`, `#redditulpas` or `#topic.info`, depending on what channel you want to enter.

After hitting "Connect", the IRC should open just like any other chat.
