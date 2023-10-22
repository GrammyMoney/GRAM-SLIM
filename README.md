# GRAM Slim

# Introduction 
**GRAM Slim** is a modular low-profile 21-button controller designed for Smash and FGC games. It has the standard pinout for firmwares like HayBox and Pico-Rectangle, and is also compatible with more fleshed-out FGC firmwares like GP2040-CE. With industrial design from GRAM, and PCB designed in collaboration with Quark.Works, this guide goes over a DIY-friendly approach to building the original GRAM Slim, and future guides/repos may hold remixes and modifications.

**If you would like to support the developer of this project, consider purchasing parts like buttons, PCBs, USB-C to GCC cables, and official GRAM builds at [GRAMCTRL.COM](https://www.gramctrl.com) rather than a fab house.**

Included Files
-
Included in this repo is all the files needed to get started with a simple GRAM Slim build:
- **GRAM Slim Frame .stl files**
- **Fab files for top and bottom panels**
- **Template DXF** for customizing top and bottom panels
- **GRAM 24mm keycap button .stl files**

Additional Information
-
If you want more info around GRAM builds, both open source and official builds, please join the [GRAM Digital Controllers Discord](https://discord.gg/6TuHw2r2X4) to ask questions and work with the community! I would love to see people creating new interesting designs, and building upon the initial framework.

Thanks & Acknowledgements
-
There are several people who made this project possible, either directly or indirectly.
- [Quark](https://twitter.com/quark_works), who did the PCB design on this and many other GRAM projects.
- [Bjart](https://twitter.com/bjartskular2), who developed the OFOF1 chassis, which was the initial development for a lot of the ideas explored in this build, including using PCB fabs for the panels, and the general idea of stacking two panels on a frame for the enclosure.
- My life and business partner [BRUISES](https://twitter.com/bruisesxo), who has turned GRAM into what it is today, and had incredible patience with me as I toiled away at my computer late into the night designing this thing.

# Ordering & Customization Guide
While most of these files are universal and can be used at any fab house, **JLCPCB** has become the de-facto standard for DIY box manufacturing. This is due to their hyper-affordable pricing and low minimum order quantity.

The PCB
-
The PCB Fabrication files should come in the form of a *Gerber ZIP file* and *bom/cpl files* (usually in Excel spreadsheet formats).

Drag them into the "Upload Gerbers" box at JLCPCB and this page will pop up:

![image](https://github.com/GrammyMoney/GRAM-SLIM/assets/126632196/399c1986-c4fd-446e-97d9-e55e6c1433eb)

Here you can change the color of the PCB. Green is the fastest and cheapest from JLC, but their black PCBs look *siiiiiick*. The only setting I recommend you change is to check "**Yes**" on *Confirm Production file*. This allows for any mistakes to be ironed out by their engineers.

Towards the bottom of the page, you want to turn on the switch for **PCB ASSEMBLY**.

![image](https://github.com/GrammyMoney/GRAM-SLIM/assets/126632196/349919ce-35f1-425e-aabc-416f8ca25363)

Make sure you are assembling the *Bottom Side* of the PCB, and make sure to set *Confirm Parts Placement* to "**Yes**". None of the advanced options need to be changed.

Upon confirming your PCB Assembly options, you'll be taken to the Assembly wizard. Clicking next will give you a location to upload the *BOM* and *CPL* files (*CPL* is referred to as *Positions* in the GRAM Slim files). Once you click through, you'll be brought to you BOM list.

![image](https://github.com/GrammyMoney/GRAM-SLIM/assets/126632196/36b6bb49-a48a-4550-983b-55a35bed7615)

This will allow you to modify parts if there's any low stock. There's a line at the bottom for CH1-CH21 with some red text. This is for assembling hotswap sockets, which is not recommended for JLC, as you have to preorder them. when you click **next**, continue by clicking *Do not place*.

![image](https://github.com/GrammyMoney/GRAM-SLIM/assets/126632196/b6534da2-4ae0-4e29-a1a3-f0b06aea3565)

The wizard looks intimidating, but good news! Since you're confirming part placement, the JLC engineers will fix any errors. Just go ahead and continue.

There you have it! Your PCB is ready to order. As of the time of this writing, a set of 5 assembled boards costs $56.07 before shipping.

The Panels
-
The process of ordering aluminum panels from JLC is similar to the PCB ordering process, but much simpler. Start by dragging the **GRAM Slim Top** Zip file into the JLC upload window. We want an aluminum PCB, 1.6mm. You can choose either white or black coating (white tends to be glossy, black is matte but a fingerprint magnet). 

![image](https://github.com/GrammyMoney/GRAM-SLIM/assets/126632196/cfec88fb-68bb-479e-8c88-61d2a660c8fc)

Under High-spec Options, make sure to remove order number, or else they'll put an ugly serial number on the panel.

Once you save to cart, you'll see this screen:

![image](https://github.com/GrammyMoney/GRAM-SLIM/assets/126632196/218c9ba4-145b-4697-92de-b3484fcedc13)

Here you can add the **GRAM Slim Bottom** Zip file, and it will copy all your settings from the Top panel. Save to cart, and you're ready to check out with your PCBs!

*Note: JLCPCB cannot transact PCB and 3D printing orders together, so place this order, then move on to 3D printing.*


The Frame
-
The frame file is pretty self explanatory. Just go into JLC's 3D printing section, drop the STL file in, and choose your material. I recommend black Resin, but LEDO 6060 is a great, low cost alternative. The only material I recommend against is the textured Nylon options, as the tolerances between the frame and panels are extremely tight, and the texture could interfere with that.


![image](https://github.com/GrammyMoney/GRAM-SLIM/assets/126632196/7fee3cdb-1453-4f1a-8c41-a377b9aa191a)


The Buttons
-
The 10x file is the ideal for JLC, as it minimizes cost. JLC may reach out to you and add some cost (0.30/pc) for small parts. This is normal.

The buttons have been tested in the same three materials:
- **LEDO 6060** (natural white, most cost-effective option, goes well with matching frame and black aluminum panels)
- **Black Resin** (matte grayish-black, goes well with both black and white panels)
- **PA12-HP Nylon** (Only slightly more expensive for buttons, but gives an amazing textured finish, very premium feel)
- **8001 Transparent Resin** (Really cool, really expensive)

# Build Guide

Building the GRAMv2 is relatively straightforward, but an updated in-depth build guide (including a video!) is currently in the works.
