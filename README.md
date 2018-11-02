# booking_bot

## Installation

You will first need to **download this repository** to your computer.
To do so, open your **Terminal app** and copy paste the following line:
```
git clone https://github.com/fabrahaingo/booking_bot.git && cd booking_bot
```

### For those who don't have Node.js and npm installed yet:
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)" && brew update && brew doctor && brew install node
```

### For everyone

Once that done, you'll need to **install all dependencies** needed for the bot to work.
Simply run:
```
npm install
```

Then **run the program** by writing:
```
node getMeATicket.js
```

A window should pop up, leading you to the folling page: [Billeterie Opera de Paris](https://billetterie.operadeparis.fr/account/login)


## Time to work for you bot, simply follow those simple steps:

**1.** Return to your Terminal.

**2.** Input your **username** then confirm.

**3.** Input your **password** then confirm.

> **NOTE**: **no character will appear** on your screen for confidentiality purposes, no worries, just hit <Enter> once you're done writing it.

![username_and_password_input](https://github.com/fabrahaingo/booking_bot/blob/master/img/credentials.png)

**4.** Go back to the opened window and **verify that you're successfully logged in**.

> **DIDN'T WORK ?** : hit Command + C and redo all the steps from "node getMeATicket.js".

**5.** In you Terminal, it's now time to tell your program which event you want to attend:
   - Simply write "**ballet**" or "**opera**" (without the brackets).
   - Then write the **name of the event** you wish to attend.
	   *For example "cendrillon"*

> **NOTE**: if the event name contains spaces, replace them all by "-".
*For example, "la dame aux camelias" will become "la-dame-aux-camelias"*.

> If the event has already been released, you'll end up with this:
![event_name_and_type_input](https://github.com/fabrahaingo/booking_bot/blob/master/img/specify_event.png)

> If the event hasn't been released yet, you'll have to wait until it finds the link. In the meantime, you'll see the number of refreshs appear continuously on your screen like so:
![wait_event_example](https://github.com/fabrahaingo/booking_bot/blob/master/img/refreshing.png)

**6.** Click one last time on the browser window

## That's it !

Sit back and relax while your bot is doing all the hard word for you.
**Don't forget to keep an eye on him** and stay ready to input the capcha you'll be asked to solve... ! :)

When you're done with your booking, click on your Terminal window and hit Command + C to kill the script.
The browser will then automatically close itself.
You can now close your Terminal.

### Features to implement:
- [ ] Capcha solver
- [X] If login fails, retries instead of having to restart the program
- [ ] Other websites that work with AJAX requests
- [ ] Check format of user inputs
- [ ] Better way to notify user when a link is found
