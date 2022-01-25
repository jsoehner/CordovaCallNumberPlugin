CordovaCallNumberPlugin

[![Git](https://app.soluble.cloud/api/v1/public/badges/3ac92ec9-8cbd-455e-960b-b3b131435180.svg?orgId=320408544746)](https://app.soluble.cloud/repos/details/github.com/jsoehner/cordovacallnumberplugin?orgId=320408544746)  
=======================

Call a number directly from your cordova application.

Install the plugin using:


``` 
npm install call-number
```

or

```
yarn add call-number
```

Use the plugin in your JS file:
``` javascript
window.plugins.CallNumber.callNumber(onSuccess, onError, number, bypassAppChooser);
```

**number:** *String;* phone number to call (e.g. "1234567890")

**bypassAppChooser:** *boolean;* true if you always wish to bypass the app chooser if user has multiple applications installed that can handle calls

Make sure to create onSuccess and onError call back functions.

Example:
``` java
function onSuccess(result){
  console.log("Success:"+result);
}

function onError(result) {
  console.log("Error:"+result);
}
```
