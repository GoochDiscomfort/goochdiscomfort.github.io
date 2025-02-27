.. title: Building a Custom Keyboard, Part 2 (Programming)
.. slug: building-a-custom-keyboard-part-2-programming
.. date: 2025-01-18 13:58:47 UTC
.. tags: Tech, Keyboards
.. category: 
.. link: 
.. description: Part 2 of my Custom QAZ Keyboard Build, this time I explain how I programmed the keyboard.
.. type: text

The Beginning
=============

After the building process, I was looking forward to actually programming and using the keyboard, however I ran into a few issues and managed to brick the whole keyboard (for a few minutes).

Firstly, I tried to use VIA, and once I had found a HID compatible browser (Chrome) I found that it didn’t work. Not sure why, but no matter what OS or browser I tried, it wouldn’t work. Then I tried to install QMK, and after reading that it was ‘slow’ on Apple Sillicon Macs, I installed it on my old Intel Macbook Air. Using Brew, a package manager for macOS, I set about installing QMK. One odd issue I encountered was Brew finding the dependancies for QMK, and compiling them from scratch. Just compiling Python 3.13 took over 40 minutes, and QMK had a lot of dependancies. If I was doing something wrong I would love to find out what it was, as the whole install process lasted overnight.

This brings us to the morning of the 12th, I sit down to a fresh install of QMK and begin trying to compile my keyboard layout. Since the QAZ uses a Raspberry Pi 2040, the Firmware files need to be converted to a .uf2 file. While it isn’t immediately clear how this is done, After some research i managed to generate a key map using QMK Configurator, and built it into a .uf2 file.

How do you upload firmware?
===========================

The photos of the PCB shows a small button on the back that is used to place the keyboard into flashing mode, but upon tearing the keyboard down I found no such button. Upon further research, I found that on RP2040 boards, you have to hold key 0,0 to put it into flashing mode. This is normally the top left key, in my case ‘Q’. After successfully placing my keyboard into flashing mode, I tentatively copied my customised firmware over to the microcontroller. After the keyboard disconnected and rebooted, I was excited to try out my custom layout. I was instead surprised to find that none of my keys worked, ‘G’ would type ’U’ and holding down ‘N’ + ‘B’ typed ‘J’. Obviously something had gone wrong somewhere in the process, but the next issue had become apparent, the new firmware had changed the keymap, and meant that I didn’t know what key 0,0 was anymore! This meant that I was unable to put the keyboard into flashing mode, nor could i actually use the nice new keyboard I had built. Luckily, I was able to dissasemble the keyboard for the 2nd time, and short the contacts where the button was supposed to be to reset the microcontroller and place it into flashing mode once again. Temporary heart attack over, I flashed the original firmware and decided to go back to square one. I sure am glad I wasted many hours installing QMK. It’s definitely something i’ll have to go back to in the future and mess round with some more. Maybe on a cheaper, properly built keyboard.

Via vs Vial
===========

Earlier on, I mentioned my attempts at using Via to program my keyboard, to no success. I had seen references to Via/Vial and had naively assumed that they were the same software, shocking news, they are not… While Via didn’t work at all, with any keyboard I tried, Vial picked the QAZ straight up and worked perfectly. Within 5 minutes, I had programmed my keyboard to do CAPITAL LETTERS, Num8er2, and Symbols!@£. Oficially, I think I wasted around 24 hours trying to program my keyboard, only to complete the whole task in the time it takes to finish a coffee. fantastic.

What layout did i Chose?
========================

At the moment, I am using 3 layers, my main alphabet keys, a numbers and symbols layer and a layer that converts my ‘wasd’ keys into arrows to move around text. I suspect I will change this quite a bit as I get used to typing on the keyboard, but for a first try this seems to work well. Challenging enough to be fun, and makes me engage my brain when working out symbols.

.. image:: /images/Layer-1.png

*My main Alpabet layer*

.. image:: /images/Layer-2.png

*Numbers and Symbols on Layer 2*

.. image:: /images/Layer-3.png

*WASD for arrow keys*

Typing on the keyboard itself is really fun, it only took a couple of days before I was able to get up to full speed (not that fast anyway). Most of this article and the last one were typed on the board, and is probably how I will write most of my blog posts from now on. In terms of sound, the board is loud enough to sound satisfying while typing, but quiet enough to not get too annoying, especially with others in the same room. It could do with some lightly taller feet at the back to give it some angle, but this is an easy fix.

For my first time building a custom keyboard it has been really fun, definitely a good starting point and very affordable. Also a surprisingly easy to use layout!

Thanks for reading, hope you’ve enjoyed following along with this. Speak to you soon!