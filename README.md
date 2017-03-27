# gettemp-promise


* This module will return the current temperature and location of the specified US Zip Code in the units requested.
* The temperature information is pulled from weather.com


## Intallation

~~~~~~~
npm install gettemp-promise
~~~~~~~

## How to use

* zipcode is a regular US postal code in numeric form
* units is specified in either Celsius or Fahrenheit as 'c' or 'f'.
* units is optional and if not specified will use the default units returned from weather.com

~~~~~~~
gettemppromise(zipcode, [units,])
  .then(function(message){
    console.log(message);
    })
  .catch(function(err){
    console.log(err);
    })
~~~~~~~

#Examples

~~~~~~~
gettemppromise(90210,'c')
  .then(function(message){
    console.log(message);
    })
  .catch(function(err){
    console.log(err);
    })
~~~~~~~

~~~~~~~
gettemppromise(30342)
  .then(function(message){
    console.log(message);
    })
  .catch(function(err){
    console.log(err);
    })
~~~~~~~
