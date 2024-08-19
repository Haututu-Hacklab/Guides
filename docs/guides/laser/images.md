# LightBurn and Images

## Loading the image

For actual image editing, like cropping or rounding corners etc, it's suggested to use something like Illustrator, GIMP, or your preferred image editing software.  
Once you have an image ready to work with in the cutter (with LightBurn), Lightburn allows you to simply drag an image into the project window and start manipulating it (in a limited amount).  

## Adjusting the image

Once an image has been loaded into LightBurn, you have a couple options.  
The most common is to do an "Image Trace", which will allow you to cut out the outline of whatever you imported. The second is to use "Adjust Image" to get it ready for 'drawing' with the laser.

=== "Image Trace"
    Once the image has been loaded, you can right-click on it and select "Image Trace".  
    This will allow you to fine tune the settings for how to outline the image you loaded, in order to either cut it out or fill it with etch.  
    To infill it (or 'colour it in'), select either "Fill" option (one fills the image itself, one fills around it).  
    To cut it out, select the "Cut" option for the tool once you've selected the line you want to cut along.  
    Always remember, cutting out the design should be the _last_ step in the process, as the work piece can move once it's detached from the main mass of the material you're using - which will mean things no longer line up for the infill.
 
=== "Adjust Image"
    Once the image has been loaded, you can right-click on it and select "Image Trace".  
    This will allow you to have the software attempt to identify details in the image itself that you can then burn in, sort of like a sketch.  
    For some pretty good details, it's suggested to use the image processing options called "Jarvis Mode" or "Stucki".  
    
    In Jarvis mode, it's suggested to use a 'Line interval' of 0.1-0.2mm, as the Hacklab laser is 0.1mm wide - going below the laser size will cause the image to look 'smeared' once it's burned.  
    In the preview window that opened, adjust the contrast and brightness options to get a nice, clear image for processing. This will adjust how much detail there is to work with. _This can take a moment to process._  
    Use "Enhance Radius"/"Enhance Amount" to really make the image 'pop' - this will adjust how much detail actually gets taken into account when shading the image with the laser itself.

## After adjusting the image

Once we've adjusted the image, the next step is to actually configure the laser settings.  
Bear in mind that we should be using high speed, low power for engraving/shading.  
Make sure that the Cut/Layer is set to "Image" mode, and then double-click it to open the cut settings.  
We want to ensure that "Air Assist" is on, and that we enable "Bi-directional scanning" (the second option helps reduce the visibility of lines on the final output). Likewise, we can adjust the "Scan Angle" to make the lines the laser uses go in different directions (rather than simply left-to-right), which can also impact the visual details in the image.

Ideally, we now also want to set our Speed and Power settings.  First, high-speed for engraving works well. This varies by material, so if you are unsure, check with someone who uses the material often. Generally, 250-350mm/sec is a good mid-speed option.
For Power, this again varies by material, so make use of the knowledge around and check with someone who has tried similar things. Ensure "Constant Power Mode" is _disabled_, as we want both Max _and Min_ options - this will allow the laser to ramp up and down on its own depending on the shade in the image. 20% can be a good option for Min on 3-4mm ply, and 40% is a pretty good option for Max on the same.

## Adding a cut command

Using the "Rectangle" tool, draw a simple box, and then adjust the Width and Height of it to the same size as the image you've just been working with.  
Then, change the XPos and YPos of it to the same as the image - this will ensure it traces around the image itself.  
With the outline selected, click on one of the tools down the bottom, and then configure it in the "Cuts/Layers" window up the top - this should be "Line" or "Cut" Mode.  
Set the power and speed for cutting the material. If it's a material that's particularly awkward, consider doing slightly lower power but a higher "Pass Count", so that it repeats the same cut a few times until the cut is done.

## Send it

That's it, done. The last thing to do is to actually line up the cut, set the origin, confirm you're framed up, and hit "Start". How to do that will be on a different page to this one, soon.
