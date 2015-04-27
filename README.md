# Learn SauceLabs

Learn to use SauceLabs.com to **Test** your
Node/Web/Mobile **apps** in ***ALL the Browsers***!

## Signup - *No Credit Card Required*

> https://saucelabs.com/signup/trial


## "*On Boarding*"

Once you have registered, you will be taken to the "***on boarding***" page:
https://saucelabs.com/docs/onboarding



### 1. Select JS


### 2. Select Copy the CURL Command


Copy-paste the CURL command that is displayed. e.g:


```sh
curl -X POST https://saucelabs.com/rest/v1/your-username/js-tests \
-u YOUR-USERNAME:SUPER-LONG-KEY \
-d platforms='[["Windows 8", "internet explorer", "10"], ["OS X 10.8", "safari", "6"]]' \
-d url="https://saucelabs.com/test_helpers/front_tests/index.html" \
-d framework=liso -d name=my-awesome-test
```

### 3. Paste & Run the CURL Command in your Terminal



## Background

+ Saucelabs *general* JS Unit Testing: https://docs.saucelabs.com/tutorials/js-unit-testing/
+ Saucelabs **Node.js** intro: https://docs.saucelabs.com/tutorials/node-js/
+ Video (by Jonathan Lipps @SauceLabs) showing testing an Express.js
app in Sauce: https://www.youtube.com/watch?v=Dzplh1tAwIg (dated; 2012!)


Watch later: https://www.youtube.com/watch?v=DO8KVe00kcU
