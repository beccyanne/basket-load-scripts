# Basket Load Scripts

## Installation
These scripts are constructed for Apache JMeter, in order to run the tests, please install JMeter from here:
http://jmeter.apache.org/download_jmeter.cgi

You can get JMeter setup using these instructions:
http://jmeter.apache.org/usermanual/get-started.html

## Opening the scripts inside the JMeter GUI
* Clone this project into your file system
* Open JMeter (generally, `./jmeter` from the bin directory of where you have JMeter installed)
* File -> Open -> Select .jmx file from cloned directory

## Thread groups
This project has a single thread group (Users). It is currently set to 1 thread with a ramp up time of 1 second.

## Running the script from command line (recommended)
From the bin directory of JMeter, you can run the following command:
`./jmeter -Jkey=<key> -Jsecret_key=<secret_key> -Jsession_endpoint=api-<env>.marksandspencer.com/v1/userprofile/guestsession? -Jbasket_endpoint=api-<env>.marksandspencer.com/basket/v2? -n -t "/<path>/add_remove_basket.jmx"`
