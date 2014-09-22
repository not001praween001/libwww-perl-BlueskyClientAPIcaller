libwww-perl-BlueskyClientAPIcaller
==================================

libwww-perl is a perl library that provides HTTP caller for perl. It is a standard library on package repository now.

You can install it easyly.

```shell

  sudo apt-get install libwww-perl

```

And use shell script for calling web API to Bluesky Server.

```shell

   #!/bin/sh
   
   edIP="Your RaspberryPI IP address."

   GPIO_PIN_NUMBER_OF_YOUR_DEFINE="3"

   BLUESKYSERVER="127.0.0.1:8189"

   GET "http://${server}/etlog?instruction=sensornetwork&opt1=${edIP}&opt2=set&opt3=d&opt4=${GPIO_PIN_NUMBER_OF_YOUR_DEFINE}&opt5=1"
   
   GET "http://${server}/etlog?instruction=sensornetwork&opt1=${edIP}&opt2=set&opt3=d&opt4=${GPIO_PIN_NUMBER_OF_YOUR_DEFINE}"

   GET "http://${server}/etlog?instruction=sensornetwork&opt1=${edIP}&opt2=set&opt3=d&opt4=${GPIO_PIN_NUMBER_OF_YOUR_DEFINE}&opt5=0"
```
