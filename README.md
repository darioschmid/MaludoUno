# MaludoUno

How to make the Maludo Uno, a single key Digispark Morse Code Keyboard mainly intended as a keychain suitable gadget.\
It runs my [Digispark Morse Keyboard](https://github.com/maludo99/DigisparkMorseKeyboard) Arduino script.

![Picture](https://github.com/maludo99/DigisparkMorseKeyboard/blob/master/Images/MaludoUno.jpg?raw=true)

## Inspiration

I was inspired by [Snipeye's Uno](https://www.reddit.com/r/mechmarket/comments/h8b27d/gb_uno_last_chance/):

![Picture](https://github.com/maludo99/MaludoUno/blob/master/Uno.jpg?raw=true)

It's based on the AtMega32u4 Microcontroller. In contrast, my "Maludo Uno" is based on the weaker, but cheaper AtTiny85/Digispark.

## My "Maludo Uno" Design

I used my [Digispark Morse Keyboard](https://github.com/maludo99/DigisparkMorseKeyboard) Arduino Script to be able to use Morse Code for Input. Previously I hardly knew any Morse Codes, but I reckoned this would be quite a fun project for getting involved into Morse Code.

### Advantages

* More cost efficient: 5 Digispark Boards are about 10€ on [Banggood](https://www.banggood.com/5Pcs-Digispark-Kickstarter-Micro-USB-Development-Board-For-ATTINY85-Arduino-p-1047665.html?rmmds=search&cur_warehouse=CN) and [Amazon](https://www.amazon.de/AZDelivery-Digispark-kompatibles-Development-ATtiny85/dp/B076KVKHH1) (incl. shipping), whereas a single AtMega32u4 board is at least 5€
* Speed Switch for adjusting the Morse Code timings
* Smaller

### Disadvantages

* No support for a RGB LED (too little available pins on the Digispark)
* Not QMK support (but full Arduino IDE support)


## How To Use It

Visit [DigisparkMorseCode/MorseCodes.txt](https://raw.githubusercontent.com/maludo99/DigisparkMorseKeyboard/master/MorseCodes.txt), or open a Text Editor and hold the key down for 4sec. It prints out all available Morse Codes.

Example:

    "M  A   L    U   D   O      U  N   O"
    "-- •- •-•• ••- -•• ---    ••- -• ---"


Setting the Speed Switch to "Fast" activates automatic space insertion between words and allows your "dah's" (long presses) to be shorter.\
If you set the switch to "Slow", you must manually add spaces between words with the morse codes "----" or "•-•••"

## How To Do It Yourself

1. Get a [Digispark](https://www.amazon.de/AZDelivery-Digispark-kompatibles-Development-ATtiny85/dp/B076KVKHH1)
2. Order the PCB (I got mine from [jlcpcb.com](https://jlcpcb.com/)). You can find the gerber files at [./KiCadFiles/GerberFiles](https://github.com/maludo99/MaludoUno/tree/master/KiCadFiles)
3. Get yourself a Cherry MX style key switch
4. (Optional) Get yourself a [MSK 12C01](https://www.ebay.de/itm/SMD-Miniatur-Schiebeschalter-Switch-Schalter-Micro-Mini-Ein-Aus-3-Pin-MSK-12C01/173613966570) SMD Switch
5. Soldering
   1. Solder Male Headers onto the Digispark (facing upwards)
   2. Solder the Speed Switch onto the PCB. This requires precise SMD soldering as the switch is tiny
   3. Solder the key switch onto the PCB
   4. Solder the PCB to the Digispark
6. Upload the code to the Digispark. Visit my [DigisparkMorseKeyboard repository](https://github.com/maludo99/DigisparkMorseKeyboard) for reference.


Feel free to improve my PCB design (e.g. add compability for other key switches). You can find the KiCad PCB Design files at [./KiCadFiles](https://github.com/maludo99/MaludoUno/tree/master/KiCadFiles).

The PCB inside KiCad looks like this:

![Picture](https://raw.githubusercontent.com/maludo99/MaludoUno/master/MaludoUnoPCBDesign.jpg?raw=true)
