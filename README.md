# zcs
A quick and light esm / node module to look up state city or zips to get either. It also has lookahead / autocomplete 

## Install

```bash

npm install zcs
```


### Node Usage 

```js

    const {  
    getByStateCity,
    getByCityState,
    getByZip,
    zipLookAhead,
    cityLookAhead,
    stateLookAhead,
    validCity,
    validState,
    validZip,
    getCitiesNameByState,
    getCitiesNameAndPopulationByState 
  } = require('zcs').zcs();
     // optional state as second param
    console.log(getByCityState('Orlando'))

     // optional city as second param
    console.log(getByStateCity('FL')) 

    console.log(getByZip('03809'))

    // optional limit as second param
    console.log(zipLookAhead('038'), 10) 
    console.log(cityLookAhead('orlan'), 5)
    console.log(stateLookAhead('N'),10)
    
    console.log(validState("FL"));
    console.log(validState("FLA"));
    console.log(validCity("Orlando"));
    console.log(validCity("OrlandFAS"));

    console.log(getCitiesNameByState("FL"));
    console.log(getCitiesNameAndPopulationByState("FL"));
```

### Web Usage


```js
 import {   
    getByStateCity,
    getByCityState,
    getByZip,
    zipLookAhead,
    cityLookAhead,
    stateLookAhead,
    validCity,
    validState,
    validZip,
    getCitiesNameByState,
    getCitiesNameAndPopulationByState
  } from 'zcs'

     // optional state as second param
    console.log(getByCityState('Orlando'))

     // optional city as second param
    console.log(getByStateCity('FL')) 

    console.log(getByZip('03809'))

    // optional limit as second param
    console.log(zipLookAhead('038'), 10) 
    console.log(cityLookAhead('orlan'), 5)
    console.log(stateLookAhead('N'),10)

        console.log(validState("FL"));
    console.log(validState("FLA"));
    console.log(validCity("Orlando"));
    console.log(validCity("OrlandFAS"));

    console.log(getCitiesNameByState("FL"));
    console.log(getCitiesNameAndPopulationByState("FL"));
```
