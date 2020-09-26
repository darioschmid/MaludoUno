# MaludoUno

How to make the Maludo Uno, a single key Digispark Morse Code Keyboard mainly intended as a keychain suitable gadget.\
It runs my [Digispark Morse Keyboard](https://github.com/maludo99/DigisparkMorseKeyboard) Arduino script.

![Picture](...)

## Inspiration

I was heavily inspired by [Snipeye's Uno](https://www.reddit.com/r/mechmarket/comments/h8b27d/gb_uno_last_chance/):

![Picture](https://i.imgur.com/OqPyWbb.jpg)

It is based on a AtMega32u4 Microcontroller. In contrast, my "Maludo Uno" is based on the weaker, but cheaper AtTiny85 / Digispark.

## My Design

I used my [Digispark Morse Keyboard](https://github.com/maludo99/DigisparkMorseKeyboard) Arduino Script to be able to use Morse Code for Input. Before I hardly knew any Morse Codes, but I reckoned this would be quite a fun project for getting involved into Morse Code.\
Check out my [Digispark Morse Keyboard repository](https://github.com/maludo99/DigisparkMorseKeyboard) to learn more.

### Advantages

* More cost efficient: 5 Digispark Boards are about 10€ on [Banggood](https://www.banggood.com/5Pcs-Digispark-Kickstarter-Micro-USB-Development-Board-For-ATTINY85-Arduino-p-1047665.html?rmmds=search&cur_warehouse=CN) and 11€ on [Amazon](https://www.amazon.de/AZDelivery-Digispark-kompatibles-Development-ATtiny85/dp/B076KVKHH1) (incl. shipping), whereas a single AtMega32u4 board is at least 5€
* Added a Speed Switch for adjusting the Morse Code timings.
* Smaller
* relatively simple programming inside the Arduino IDE. A little [setup](https://digistump.com/wiki/digispark/tutorials/connecting) is required.<sup>(*)</sup>

### Disadvantages

* No support for a RGB LED, because the Digispark has simply too few available pins
* 
* Not QMK compatible (AtTiny has no native USB support)


<sup>(*)</sup> Warning: only get involved into changing fuses if you know what you are doing, you can easily brick your DigiSpark (Trust me, I have). You can savely ignore this if you don't know what I#m talking about.



## Operation



## A

## KiCad PCB Design

You can find the KiCad PCB Design files aswell as the gerber files at [./KiCadFiles](https://github.com/maludo99/MaludoUno/tree/master/KiCadFiles).

Here is a screenshot:

![Picture](https://raw.githubusercontent.com/maludo99/MaludoUno/master/MaludoUnoPCBDesign.jpg?raw=true)
