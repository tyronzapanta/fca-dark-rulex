## Notification !

Note! This Is The Main Chat Api Product By [Facebook-Chat-Api](https://github.com/Anupx0/Anupbot) Lead Author: [Anup Kumar](https://github.com/Anupx0), Current Author Not Responsible! ), If Yes Error Try Using Another Product !

## Support For : 

+ Support English, VietNamese !,
+ All bot if using listenMqtt first.

# Api For ChatBot Messenger

Facebook Already Has And For Users To Create Api For Chatbots At Dey => [Here](https://developers.facebook.com/docs/messenger-platform).

### This Api Can Make You Payy Acc Like You Never Have, Please Pay Attention =))

Note ! If You Want To Use This Api Please See The Document At [Here](https://github.com/Anupx0/Anupbot).

## Download

If You Want To Use It, Download It By:
```bash
npm i inopen-test
```
or
```bash
npm inopen-test
```

It Will Load Into node_modules (Your Lib) - Note Replit Won't Show Where to Find

### Download Latest Version Or Update

If You Want To Use The Latest Version Or Update Then Go To Terminal Or Command Prompt Enter :
```bash
npm install inopen-test@latest
```
Or
```bash
npm i inopen-test@latest
```

## If You Want To Test Api

Benefits For This You Will Not Spend Time Paying Acc And Have Acc
Use it with a Demo Account => [Facebook Whitehat Accounts](https://www.facebook.com/whitehat/accounts/).

## Using

```javascript
const login = require("inopen-test"); // get it from the lib

// log in
login({email: "Gmail Account", password: "Your Facebook Password"}, (err, api) => {

    if(err) return console.error(err); // error case

    // tạo bot tự động nhái theo bạn:
    api.listenMqtt((err, message) => {
        api.sendMessage(message.body, message.threadID);
    });

});
```

As a result, it will copy you as shown below:
<img width="517" alt="screen shot 2016-11-04 at 14 36 00" src="https://cloud.githubusercontent.com/assets/4534692/20023545/f8c24130-a29d-11e6-9ef7-47568bdbc1f2.png">

If You Want Advanced Use Then Use Bot Types Listed Above !

## List

You Can Read Full Api At => [here](DOCS.md).

## Install For Anup:

You need to go to file Anup.js, Then Find Line
```js
    var login = require('inopen-test'); 
    /* Maybe :
        var login = require('fca-anup');
        var login = require('fca-aliya-anup');
        var login = require('aliya-anup');
    ...   
    */
```

And Replace It With:

```js
    var login = require('fca-dark-rulex')
```

Then Run As Normal!

### Save Login Information.

To Save You Need 1 Apstate Type (Cookie, etc,..) To Save Or Use Login Code As Above To Login !

And This Mode Is Available In Some Bots In Vietnam So You Can Rest assured!

__Guide With Appstate__

```js
const fs = require("fs");
const login = require("inopen-test");

var credentials = {email: "FB_EMAIL", password: "FB_PASSWORD"}; // tk information

login(credentials, (err, api) => {
    if(err) return console.error(err);
    // log in
    fs.writeFileSync('appstate.json', JSON.stringify(api.getAppState(), null,'\t')); //create appstate
});
```

Or Easier (Professional) You Can Use => [c3c-fbstate](https://github.com/c3cbot/c3c-fbstate) To Get Fbstate And Rename It To Apstate Is Also ! (appstate.json)

------------------------------------

## FAQS

FAQS => [Link](https://github.com/Anupx0/Anupbot#FAQS)
