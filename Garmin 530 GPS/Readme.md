# Garmin 530 GPS Unit

In this directory, you'll find the files required to build your own fully functional Garmin 530 GPS unit for use with X-Plane and Microsoft Flight Simulator 2020.  I use this unit successfully with both X-Plane 11 and 12, and it also works seamlessly with FS 2020.  With the exception of a few purchased electronic components and one piece of software, all parts for this unit are 3D printed out of standard PLA filament.

This unit interfaces with your simulator via an Arduino 2560 connected to your PC via a USB cable. Software interaction is handled completely through SimInnovations' Air Manager application.

## General overview of construction steps

Once the unit is assembled (details on that are contained in a separate instruction file), the general steps to get it working are as follows (details on each process will be provided):

1.  Install Air Manager on your simulator PC.
2.  Load the Air Manager firmware on the Arduino 2560.
3.  Add the Garmin 530 Hardware item to your Air Manager instrument panel.
4.  Map the buttons and encoders to their associated pins on the Arduino 2560.
5.  Provide power to the 5" HDMI display in the unit and connect as a display on to your PC.

## Bill of Materials for Electronics Required

Aquire the following components you'll need for the build.  Vendor links are provided where I purchased them:

1.  Dual Encoder from PropWash Simulations for your COM/NAV and GPS control encoders.
    You'll need two of these, they run $12.95 each.  
    https://www.propwashsim.com/store/dual-encoder-kit
    
2.  6mm Tactile Push Button Assortment.  Way more than you need for this one project,
    but you'll use them in lots of components in this project!  Runs about $10 on Amazon.
    https://www.amazon.com/gp/product/B071KX71SV/ref=ppx_yo_dt_b_asin_title_o05_s01?ie=UTF8&psc=1
    
3.  10k Ohm potentiometers for your volume knobs.  Again, buy this assortment, because
    you'll use these in your yoke controller and for other instruments as well.  $10 on Amazon.
    https://www.amazon.com/gp/product/B09897HR3C/ref=ppx_yo_dt_b_asin_title_o06_s00?ie=UTF8&psc=1
    
4.  INNOLUX 5.0inch 640x480 TFT LCD Panel Display with ZJ050NA-08C 50Pin TTL Driver Board.
    Purchased this on Ebay.  There are several models of this available, just be sure you get
    one similar to this, as it's a perfect fit.  Runs about $60.
    https://www.ebay.com/itm/144602928596
    
Once you have all of your parts required for the build, You're ready to 3D print your housing and assemble your unit. I am currently filming a detailed assembly video, which I will post as soon as it's available.  In the meantime, here are the general steps:

1.  3D print the parts in this directory.  I recommend using black PLA filament, as it most closely resembles an actual Garmin unit.
2.  You'll hot glue the 6mm momentary push buttons into the square sockets on the main support frame.
3.  Lettering on the buttons and on the faceplate are raised - I recommend taking your time and painting the letters with standard 
    white model paint.  Keep your brush dry except for the tip, use a magnifying lamp, and they turn out great.  If you so desired,
    you could print the faceplate in WHITE PLA, then paint it matte black and carefully use sandpaper to expose the white lettering.
    Go with whichever method works best for you.
4.  Install your volume potentiometers into their respective slots.  You might need to trim a little with a Dremel to get them to fit,
    as the housings can vary just a bit depending on where they were made.  Secure them to the frame with hot glue - simple and effective.
5.  Assemble and install your dual encoder units.  The small nut on the stem will secure the faceplace to the housing.
6.  Install the 5" display - I suggest plugging it up to your computer to ensure you know which way is up and down.  Nothing more
    aggravating than to get it secured in place only to have to disassemble it again later!  (Yeah, I did that.)  Secure it with
    either the 3D printed clips or you can use hot glue, again, at the corners and sides.
7.  now comes the fun part.  Take your time, and with a good quality soldering iron, follow the wiring diagram provided to wire up your
    unit.  In a nutshell:
    - For the buttons:  There are four pins on each one.  You only need to use one side.  One leg to ground, the other to a digital pin
      on the Arduino. Suggestion:  Wire all of the grounds in series, so you only have one leg to ground for all buttons.
    - For the volume pots:  Left pin to 5v, middle to analog pin on the Arduino, Right to ground.
    - For the encoders:  Five pins on each.  1 to 5v, 1 to ground, and three go to digital pins (one for the inner encoder, one for 
      the outer encoder, and one for the push button.
8.  Once your soldering is done, use a small dab of hot glue to attach your 3D printed buttons to the face of the push buttons mounted in your unit's frame.  Just a small dab is all that you need.  This works well, as should you ever need to replace a button, you can pop them off without damaging the electronic button below.
      
## Arduino Notes

Which pins you use on the Arduino are entirely up to you.  You're only going to have four different types of connection for each component:
- 5V pin where power is needed.  (pots and encoders usually need this.)
- Ground pin for all components.
- Digital pin (D1,2,3, etc.) for encoders, push buttons, LED displays, and other digital inputs.
- Analog pin (A1,2,3, etc.) for potentiometers and other analog components.

Once everything is wired up to your computer, you simply need to go into Air Manager and add the Garmin 530 Hardware item to your instrument
panel. (I'll cover this process in a separate video.)  Once you add it, you'll select the GPS and then assign the pins you've connected
for each button and control so that Air Manager knows what inputs to look for for each signal.  It will then work its magic and send all
of these inputs to your simulator when you use them.   Again, I will cover this process in great detail in a video coming soon.

## How does the Garmin 530 screen in the sim display on my unit?

As most of you already know, you can 'pop out' the 530 and 430 display screens in both X-Plane and FS 2020.  Once you pop these out, you
simply drag the window to the 5" display on your new GPS unit.  X-Plane will remember its location automatically for each aircraft.  I 
recommend using the free Popout Panel Manager utility to do this for FS 2020, as it's a bit more tedious to pop them out manually.
You can find a link for this utility in my general overview video in my Youtube library.

As noted, I'm just now getting all of this information assembled, but these are the main parts you'll need to start construction.  Look for more updates shortly, and if you have any questions at the moment, please feel free to contact me at my public email address on my Github profile.

**Happy building!**

*-Scott
2/10/2023*

    
