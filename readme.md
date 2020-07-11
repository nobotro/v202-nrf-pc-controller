## wltoys-v202-micropython

This  project is full functional implementation of wltoys v202 protocol,specified for rc cars A959, A969, A979 in micropython using nrf24l01 and  esp32.
Project don't need any modification of car or stock controller


## Usage
- Put "main.py", "rc.py","regs.py" and "server.py" in esp32 board with micropython firmware
- Connect nrf pins correctly(we use software spi) 'miso': 32, 'mosi': 33, 'sck': 25, 'csn': 26, 'ce': 27
- Run "remote.py" in your pc and connect esp32's wifi
- Key 'w'-go forward,'s'-go backward,'a'-steer left,'d'-steer right'
    </br>key.up-increase gear,key.down-decrease gear,key.left-steer trim,key.right-steer trim
- It has 4 speed level .you can modify gears and steering sensitivity in "server.py" 
- Wifi access point name is "ESP-carr" with no password


## Demontration video 
https://www.youtube.com/watch?v=3xs4lEP5NvE

## Used resurces 
 - https://github.com/execuc/v202-receiver/blob/master/v202_protocol.cpp
 - https://github.com/goebish/nrf24_multipro/blob/master/nRF24_multipro/V2x2.ino
 - https://bitbucket.org/rivig/v202/src/default/

[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=kevlishvilimisha1@gmail.com&lc=US&item_name=Tm8gbWF0dGVyIHdoYXQgcGVvcGxlIHRlbGwgeW91LCB3b3JkcyBhbmQgaWRlYXMgY2FuIGNoYW5nZSB0aGUgd29ybGQ=&no_note=0&cn=&currency_code=USD&bn=PP-DonationsBF:btn_donateCC_LG.gif:NonHosted)