opengrapher
===========

A Node module to parse Twitter metadata from a webpage.

[![Build Status](https://travis-ci.org/z4r/opengrapher.svg?branch=master)](https://travis-ci.org/z4r/opengrapher)


How To Install
--------------

    npm install opengrapher
    
How To Use
----------

```javascript
var opengrapher = require('opengrapher');

opengrapher.parse('http://ogp.me/', function(err, og) {
    if (err) throw err;
    console.log(og);
});
```

__output__:
```javascript
{ card: 'photo',
  title: 'imgur: the simple image sharer',
  image: 'http://i.imgur.com/mOvs78u.png',
  'image:width': '550',
  'image:height': '500',
  description: 'Mr. Nervous!',
  site: '@imgur',
  domain: 'imgur.com',
  'app:id:iphone': '639881495',
  'app:id:ipad': '639881495',
  'app:id:googleplay': 'com.imgur.mobile' }
```
