# Learn SauceLabs [![Sauce Test Status](https://docs.saucelabs.com/images/reference/status-images/status-passing.3a137816.png)](https://saucelabs.com/u/nelsonic)


> ***No Prior Experience Necessary***!

## Why?

Giving the ***people using your web/mobile app*** a ***great
experience*** is the key to ***happiness***.  
If you fail to find (and fix) the bugs in your project,
because you did not test it in the target devices/browsers,
everyone will be sad ...
so take ***20 mins*** to learn about SauceLabs ***Today***!

## Who?

***Everyone*** writing web or mobile applications *should*
be testing.

## What?

SauceLabs.com lets you **Test** your
Node/Web/Mobile **apps** in ***ALL the Browsers***!

![saucelabs homepage features](http://i.imgur.com/e6kRatE.png)

If you have never *heard* of SauceLabs, or need a refresher,  
take a couple of minutes to read their list of features:
[saucelabs.com/**features**](https://saucelabs.com/features)

## How?

### Signup - *No Credit Card Required*

First thing you will need to do is signup for the service.
Its *free*. (You will only be asked )

> https://saucelabs.com/signup/trial

![register for saucelabs](http://i.imgur.com/5f5IOvO.png)

### "*On Boarding*"

Once you have registered, you will be taken to the "***on boarding***" page:
https://saucelabs.com/docs/onboarding  
Chose ***Automated***.

![click on automated tests](http://i.imgur.com/WsMD5DQ.png)

Next you will see a few **programming language options**

### 1. Select JS

![select javascript](http://i.imgur.com/2E1aqTV.png)


### 2. Copy the CURL Command

Copy the CURL command that is displayed (into your clipboard)

![Imgur](http://i.imgur.com/DPYkAtA.png)


### 3. Paste & Run the CURL Command in your Terminal

Paste the CURL command you just copied in the previous step
into a Terminal window and press the enter key to run the test:

![curl command results](http://i.imgur.com/071Qy6V.png)

### 4. View the Results in the Browser

Once you have run the command in your terminal,
you can view the *results* in the browser.  
visit: [saucelabs.com/**account**](https://saucelabs.com/account)  
You should expect to see a list of the tests that have been run:

![list of past tests](http://i.imgur.com/ddmrzFI.png)

***Click*** on one of the tests to view the result. e.g:

![Imgur](http://i.imgur.com/fPYCUfq.png)


### 5. Watch the *Video* of the test you just ran!

![watch the video of your test](http://i.imgur.com/wKq5rVD.png)

## *Explanation*

Ensure you understand the command you just ran in the terminal:

```sh
curl -X POST https://saucelabs.com/rest/v1/USERNAME/js-tests
-u USERNAME:SAUCELABS-UNIQUE-KEY
-d platforms='[["Windows 8", "internet explorer", "10"], ["OS X 10.8", "safari", "6"]]'
-d url="https://saucelabs.com/test_helpers/front_tests/index.html"
-d framework=jasmine
-d name=sauce-sample-test
```

+ `curl -X POST https://saucelabs.com/rest/v1/USERNAME/js-tests` - ***send*** a **POST request** to this REST endpoint specifying the **JS Test** we want to run.
+ `-u USERNAME:SAUCELABS-UNIQUE-KEY` - ***authenticate*** with your **Username** and **SauceLabs Key**
+ `-d platforms='[["Windows 8", "internet explorer", "10"], ["OS X 10.8", "safari", "6"]]'` - ***specify*** which **Operating System** and **Browser Version** you want to run your test in.
+ `-d url="https://saucelabs.com/test_helpers/front_tests/index.html"` - **url** you want SauceLabs to test.
+ `-d framework=jasmine` - the ***testing framework*** you want to run for this test
+ `-d name=sauce-sample-test` - ***name*** of the test you are running (*any string is valid*)

### Notes:

+ While the [***JS*** *tutorial*](https://docs.saucelabs.com/tutorials/js-unit-testing/)
on SauceLabs *instructs* you to
setup **Karma** *and* use **Mocha**,  
these are by no means the only options for tools.
+ ***Other***  (front-end) JavaScript testing frameworks are supported: including **QUnit**, **Mocha**, **Jasmine** and **YUI**.
+ It is not immediately *obvious* in the docs, but in *addition* to these existing frameworks,  
you can also write ***custom*** tests:
https://docs.saucelabs.com/reference/rest-api/#js-unit-testing

## Conclusion

***That's it***! Now you know how to run a **Cross-Browser Test** on SauceLabs!

[![Sauce Test Status](https://saucelabs.com/browser-matrix/kimmobrunfeldt.svg)](https://saucelabs.com/u/nelsonic)


### What's *Next*?

+ ***Explore*** the other features SauceLabs has to offer:
[saucelabs.com/**features**](https://saucelabs.com/features)
+ ***Star*** this repo/tutorial (on GitHub!) to show others you liked it!
+ ***Tweet us*** if you want a ***more advanced tutorial***!

## Background

+ Sacelabs JavaScript Testing: https://saucelabs.com/javascript
+ Saucelabs *general* JS Unit Testing: https://docs.saucelabs.com/tutorials/js-unit-testing/
+ Saucelabs **Node.js** intro: https://docs.saucelabs.com/tutorials/node-js/
+ ***Video*** (by Jonathan Lipps @SauceLabs) showing testing an Express.js  
app in Sauce: https://www.youtube.com/watch?v=Dzplh1tAwIg (dated; 2012!)

### Node.js Module

SauceLabs *recommends*: https://github.com/holidayextras/node-saucelabs  
(hasn't been updated in a while, but has no dependencies so should be fine)

### Saucelabs Browsers

The ***full list*** of *available* ***platforms and browsers*** is: https://saucelabs.com/platforms/  
An example configuration file: http://git.io/vfAMY
