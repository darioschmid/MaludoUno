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
Go to [Digispark Morse Keyboard](https://github.com/maludo99/DigisparkMorseKeyboard) for the software side of things.

### Advantages

* More cost efficient: 5 Digispark Boards are about 10€ on [Banggood](https://www.banggood.com/5Pcs-Digispark-Kickstarter-Micro-USB-Development-Board-For-ATTINY85-Arduino-p-1047665.html?rmmds=search&cur_warehouse=CN) and 11€ on [Amazon](https://www.amazon.de/AZDelivery-Digispark-kompatibles-Development-ATtiny85/dp/B076KVKHH1) (incl. shipping), whereas a single AtMega32u4 board is at least 5€
* Added a Speed Switch for adjusting the Morse Code timings.
* Smaller

### Disadvantages

* No support for a RGB LED, because the Digispark simply has too little available pins
* Not QMK compatible (AtTiny has no native USB support)


## Operation

Visit [DigiskarkMorseCode/MorseCodes.txt](https://raw.githubusercontent.com/maludo99/DigisparkMorseKeyboard/master/MorseCodes.txt), or open a Text Editor and hold the key for 5sec. It prints out all available Morse Codes.

Example:
```
"M  A   L    U   D   O      U  N   O"
"-- •- •-•• ••- -•• ---    ••- -• ---"
```

Setting the Speed Switch to "Fast" activates automatic space insertion between words and allows your "dah's" (long presses) to be shorter.\
If you are in "slow Speed Mode", you must manually add spaces using the morse codes "----" or "•-•••"

Now you can start morsing!

## KiCad PCB Design

You can find the KiCad PCB Design files aswell as the gerber files at [./KiCadFiles](https://github.com/maludo99/MaludoUno/tree/master/KiCadFiles). The PCB wil look like this:

![Picture](https://raw.githubusercontent.com/maludo99/MaludoUno/master/MaludoUnoPCBDesign.jpg?raw=true)
