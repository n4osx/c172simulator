Garmin 530 GPS Unit

In this directory, you'll find the files required to build your own fully functional Garmin 530 GPS unit 
for use with X-Plane and Microsoft Flight Simulator 2020.  I use this unit successfully with both
X-Plane 11 and 12, and it also works seamlessly with FS 2020.  With the exception of a few purchased
electronic components and one piece of software, all parts for this unit are 3D printed out of 
standard PLA filament.

This unit interfaces with your simulator via an Arduino 2560 connected to your PC via a USB cable.  
Software interaction is handled completely through SimInnovations' Air Manager application.

General overview of construction steps:

Once the unit is assembled (details on that are contained in a separate instruction file), the
general steps to get it working are as follows (details on each process will be provided):

1.  Install Air Manager on your simulator PC.
2.  Load the Air Manager firmware on the Arduino 2560.
3.  Add the Garmin 530 Hardware item to your Air Manager instrument panel.
4.  Map the buttons and encoders to their associated pins on the Arduino 2560.
5.  Provide power to the 5" HDMI display in the unit and connect as a display on to your PC.

Bill of Materials for Electronics Required:

Aquire the following components you'll need for the build.  Vendor links are provided where
I purchased them:

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
    
    
