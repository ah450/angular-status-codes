# angular-status-codes
HTTP status code constants for angular

##Installation
`bower install angular-status-codes`

##Usage
```javascript
var app = angular.module('myApp', ['httpStatusCodes'])

app.controller('MyController', function($http, httpStatusCodes) {
  $http.get('/something')
   .catch( function(response) {
    if (response.status == httpStatusCodes.BAD_REQUEST) {
      // Do something
    }
   });
})
```
