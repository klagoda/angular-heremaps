[![Build Status](https://travis-ci.org/dverbovyi/angular-heremaps.svg?branch=master)](https://travis-ci.org/dverbovyi/angular-heremaps) [![Test Coverage](https://codeclimate.com/github/dverbovyi/angular-heremaps/badges/coverage.svg)](https://codeclimate.com/github/dverbovyi/angular-heremaps/coverage)

# angular-heremaps
*Live demo* **https://dverbovyi.github.io/angular-heremaps/**

Angular directive for working with Nokia Here Maps

### Install guide:

        npm install angular-heremaps

#####include angular-heremaps file

```html
    <script src="/node_modules/angular-heremaps/dist/angular-heremaps.js" type="text/javascript"></script>
```
    
#####add dependency in your angular application

```javascript 
    angular.module('exampleModule', ['heremaps'])
```
        
#####add config provider:
Before, you should register [here](https://developer.here.com/plans/api/consumer-mapping) and get your app id. Then pass it below

```javascript
    angular.module('exampleModule')
        .config(["HereMapsConfigProvider", function(HereMapsConfigProvider) {
            HereMapsConfigProvider.setOptions({
                'app_id': 'your_app_id_here',
                'app_code': 'your_app_code_here',
                'useHTTPS': true
            });
        }]);
```

####Simple directive initialization with default options.

```html
        <div heremaps></div>
```

See details on [wiki pages](https://github.com/dverbovyi/angular-heremaps/wiki)

Please report, any issue [here](https://github.com/dverbovyi/angular-heremaps/issues)
