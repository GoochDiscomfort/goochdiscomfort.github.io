.. title: My First Time Building A Custom Keyboard (QAZ!)
.. slug: my-first-time-building-a-custom-keyboard-qaz
.. date: 2025-01-13 13:17:10 UTC
.. tags: 
.. category: 
.. link: 
.. description: In this post, I detail my experience buidling a custom QAZ Layout Mechanical Keyboard
.. type: text

Introduction
============

In this post, I will document my experience custom building my first ever Custom Mechanical Keyboard, A QAZ layout sub 40%. This post will focus on building the keyboard, I will release a follow up post talking about my experience programming and using the keyboard later.

This project came about while I was looking at redoing my desk/workspace. I was thinking of going for a small mechaincal keyboard, 60% or smaller. Having previously used both a TKL (Keychron C3 Pro) and a 60% (Keychron K3) I found that I liked the idea of a smaller keyboard as it freed up a lot of desk space, and looked tidier. I was also interested in buidling a custom keyboard and the experience of customising the keyswitches and caps, really being able to fine tune the sound and feel of the keyboard.

With this in the back of my mind for a while, I stumbled across a Reddit post of someone showing off their new ‘QAZ’ keyboard. This ignited my curiosity, and after a few days of research, I had a QAZ PCB on order and had begun planning my first custom mechanical keyboard.

While the idea of a QAZ layout might seem strange and inconvinient at first, I think it looks likle a lot of fun, having to program it and really think about what you're typing and how you do it.

.. raw:: html

    <embed><blockquote class="reddit-embed-bq" style="height:500px" data-embed-height="660"><a href="https://www.reddit.com/r/CustomKeyboards/comments/1hmrstq/qaaaazzz/">Qaaaazzz</a><br> by<a href="https://www.reddit.com/user/dbsds87/">u/dbsds87</a> in<a href="https://www.reddit.com/r/CustomKeyboards/">CustomKeyboards</a></blockquote><script async="" src="https://embed.reddit.com/widgets.js" charset="UTF-8"></script></embed>


Parts List & Why I chose them


.. list-table:: Parts List
    :widths: 75 25
    :header-rows: 1

    * - Item
      - price
    * - PCB - CBKBD QAZ V2 Hotswap 
      - £28
    * - Switches - Gateron Oil King (4 Packs of 10) 
      - £26
    * - GMK Screw In Stabiliser (2x 2U)
      - £5
    * - M2x5mm Standoffs (10) 
      - n/a
    * - M2x6mm Machine Screws (Pack of 100)
      - 
    * - M2 Brass Washer (Pack of 100) 
      - 
    * - 12.7x3.5mm Rubber Feet (Pack of 24)
      - 
    * - Vintage Sytle Apple Macintosh Keycaps
      - £17

PCB
---

I bought my PCB from KeebSupply, the EU supplier for Coffe Break Keyboards (CBKBD). I chose the Hot-Swap version of the board as I didnt want to risk testing out my soldering skills on this project. Shipping from KeebSupply was quite fast from Germany to the UK, and the PCB came well packaged.

Switches
--------
From my previous experince with the Keychron K3 using Low Profile Gateron Red Switches, I knew I wanted linear switches as opposed to tactile or clicky. The one element of the K3 that I disliked was the low profile of the switches and caps. With this in mind I decided to go for the Gateron Oil King, which got good feedback and seemed like a well regarded switch. I also liked the sound of them from the typing tests I had seen online. I ordered from Mechboards in the UK, and the shipping was very quick and the items were well packaged (they even included a cool sticker).

Stabilisers
-----------
I didn't put very much thought into the stabilisers, I just went for whatever Mechboards had in stock. I can't imagine you can go too badly wrong with stabilisers.

Keycaps
-------
I had initially planned to use a set of GMK Clone Thinkcaps, in the theme of an old IBM Thinkpad Keyboard. When they arrived I decided that I actually wanted to use them on my other keyboard (Keychron C3), so I decied to get a cheap set of 'Macintosh' styled caps instead. They also have a cool retro vibe to them and feel suprisingly good!

Additional Parts
----------------
I chose the additional parts for assembely (Standoffs, Washers, Bolts and Feet) based purely off of what was available from Farnell. As I find out later, these were far from ideal. The quality and packaging was top notch, but i could've done a better job selecting them. I've given some recommendations later on as to what you should order if you decide to do this yourself.

The Build
=========

.. image:: /images/IMG_6591.jpg

Case 3D Printed on a Creality Ender V3 using black PLA+ (Design by Dingus McGee)

The first part I obtained was the case, as this was easily 3D printed at home. I used my Creality Ender V3 and printed at the ‘Optimal’ speed using Creality PLA+. The print came out really nice, with no obvious issues. I decided to start off with the ‘No Handle’ case, but I might print off the case with the handle for fun, maybe in a different colour.

The first issue I encountered was the standoffs, despite ordering the shortest available, they were far too long too long and went straight through the case leaving them a bit loose. Luckily, I was able to trim them down and make them fit. While they have a little bit of play, when the keyboard is on the desk it feels very solid, and only shifts if you try and move it. This could be solved by making the bottom of the case slightly thicker or by adding nuts to the bottom but isn't particularly needed.

Then I placed the PCB into the case, it fit perfectly but the 6mm Machine Bolts were a bit too long. I was able to stack up 7 washers onto the bolts to secure it, but I would definitely recommend using shorter bolts especially if you need to disassemble the board for troubleshooting. Probably around 3-4mm would work best.

Next, I added the stabilisers for the space and backspace keys along the bottom row. Initially these were quite stiff, and in lieu of proper lubricant, a few drops of 3-IN-ONE worked well enough. Maybe at some point I’ll take the board apart and properly lube them. Mechboards did offer a pre-lubricating service which I would definitely consider using in the future.

Luckily, after these small issues, the rest of the build went perfectly. All of the switches went in perfectly, i’m really happy with the sound of the oil kings, very clunky and smooth. The space and backspace buttons with the stabilisers don’t feel perfect, but i’m happy to live with them for a first try.

Once I was finished I plugged the Keyboard straight into my laptop and got to typing, this article in fact! The split space/backspace keys were picked up straight away. No way of typing numbers or symbols, but all it needs is some simple programming (more of this 'simple' process in the next post...)

.. image:: /images/qaz-keb.jpeg

Well, I hope you enjoyed this small post on my QAZ build, and I hope it helps you if you’re thinking of building your own. I would really reccomend it, as it has been a very fun process and an affordable way to learn the basics of building custom keyboards. I'm already researching the next keyboard I want! As I mentioned, the next post will cover my experience programming the keyboard and my thoughts after using it for a few days.