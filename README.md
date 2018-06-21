# Data gifs

In this workshop we will prepare a GIF for use on social media using SVG Crowbar, Photoshop and Illustrator.

## Requirements

* Chrome
* [SVG Crowbar 2](https://nytimes.github.io/svg-crowbar/)
* Photoshop
* Illustrator
* QuickTime player

## Storytelling with Illustrator & Photoshop

1.  Check this snazzy [house price interactive](https://www.economist.com/graphic-detail/2018/02/09/the-economist-house-price-indices)

2.  Use SVG Crowbar, just click on the bookmark
    * Find the right .svg file and download it
    * Open in illustrator
    * Turn background white
    * Play around with it
    * Create a layer for every frame with your highlights and annotations
    * Save a png for each one of those layers. This will keep the file size down (very important for gif-making)

3.  Open one of the files in Photoshop, add the other one as a new layer

4.  Create a frame animation with both files
    * Select the "Window" tab and tick "Timeline"
    * Click on the "Create Frame Animation" in your new timeline at the bottom of the window
    * Go to the menu button (the four lines in the top right corner of the timeline) and select "Make Frames from Layers"
    * Now all your layers are frames in your timeline and you can select how long each frame will be shown for and get them in the right         order
    * Save it as a gif by clicking “File” -> “Export” -> “Save for Web”
    * Select GIF in the top right corner
    * Play around with “Lossy”, “Dither” and “Web snap” and see how it changes the preview
    * Make sure “Looping options” are set to forever
    * Click “Save” (not “Done”)
    * Et voila. You’ve created your first data gif, congratulations!
    * Look at it in different browsers, on your computer, on slack. Notice any differences?

5.  Now you’ve got a self-made .gif showing the chart in a unique way for social media. You could use a template with it, add text and so on and so forth

## Recording with QuickTime

1.  Open [this interactive](https://www.economist.com/graphic-detail/2017/12/25/china-is-still-a-toy-manufacturing-powerhouse) in Chrome, have a look at it

    * Right click on the bubble chart
    * Select ‘inspect element’
    * Look at the source code and find a link that leads to the interactive
    * Hint: It’s in an iframe
    * https://infographics.economist.com/2017/toy-trade/ there we go
    * You can now change the size of the window and if you reload the page the chart will resize

2.  Open QuickTime player, do a screen recording of the bubble chart

    * Click on “File” and select “New screen recording”
    * Click on the red recording button
    * Click and drag to record part of the screen
    * Select the area of the chart
    * Now you can open the Developer Tools and remove different elements to have a clean canvas
		* Remove the divs with the classes `.interactive-header` and `.toggle-bar`
		* With the DevTools open find the span with the class `.year` and add the following styles
```
position: absolute;
margin-left: auto;
margin-right: auto;
left: 0;
right: 0;
top: 40px;
````
	  * Find the div with the class `.restart` and add the following styles
```
position: absolute;
margin-left: auto;
margin-right: auto;
left: -95px;
right: 0;
top: 40px
opacity: 0;
````
		* Now the icon to restart the graphic is hidden but you'll be able to click it anyway.
    * Click on the hidden restart icon and start recording (a good resolution if your screen is big enough is 1920x1080)
    * When done, click on the QuickTime icon on the tray and select ‘Stop screen recording’
		* Click on "Edit" and "Trim" and you'll be able to cut the video as you wish
    * Save the video

3.  Open Photoshop
    * Select “File” -> “Import” -> “Video frames to layers”
    * Select the range you want by using the sliders below the preview limit to every 2 frames (it will get more shroppy, but the file           size will decrease if you choose less frames. It will cut off after - 500 frames anyway. You can manually delete frames later as           well)
    * Click “Window” -> “Timeline”, a timeline will pop up below your normal preview. The timeline shows all layers, now converted to -         frames like in a video (or gif!)
    * Select a time period you want the first frame to be shown for (some web pages will automatically show the first frame of a gif for         at least at least second, but this differs). You can just change the time underneath each frame
    * If you want to change the time for all frames, you can click on the first, hold down shift and select the last. Now you can change         the time on any of the frames and it will change for the others as well
     * Save it as a gif by clicking “File” -> “Export” -> “Save for Web”
    * Select GIF in the top right corner
    * Play around with “Lossy”, “Dither” and “Web snap” and see how it changes the preview
    * Make sure “Looping options” are set to forever
    * Click “Save” (not “Done”)
   
