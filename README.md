This is my contribution to the "skinning" or otherwise reproducing the look and feel of classic Mac OS System 1–7 and HyperCard in websites and other modern media.

The icons here are reproduced from the 1-bit icons as vectors each pixel in the 1-bit graphic starts as a 1x1 pixel vector. Therefore, the resulting svg are scalable without being dithered by browsers or losing eh 1-bit apprearance.

The fonts are all TrueType and woff/woff2 conversions from the 1-bit files. They can be used in desktop applications to emulate the 1-bit fonts or used as @font-face references in websites.

Here's the workflow I got to work to convert a "suitcase" from an iMac G4 that has Mac OS 9.2 installed alongside OS X 10.4.11 Tiger.

While booted into OS X, I opened the OS 9 System folder and the Fonts folder. I simply copied a font file (Palatino, for example) onto a USB stick. 

I then mounted the USB stick on my MacBook Pro running macOS 15. Using DfontSplitter, I opened the font file from the iMac. DfontSplitter pulls out all the bitmap fonts as .bdf files as well as the ttf files that are the curve versions of the font.

I opened the .bdg files in FontLab 8 and saved them all as .ttf files.

Finally to make them all web-ready I converted these new bitmap .ttf files using https://transfonter.org to get .woff and .woff2 files.

**Caveat!** This pipeline probably won't work for font files older than OS 9 or so that are not hybrid bitmap and .ttf fonts. This file format doesn't get stripped of the resource fork when copying from an old Mac to a new one, thus DfontSplitter can open it.

