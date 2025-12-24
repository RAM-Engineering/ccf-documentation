by Blake!

In this demo I'll be designing and fabricating my first microfluidic chip. 

Here is an awesome resource to use btw!
https://www.youtube.com/@dk-hu3er/videos

Things to do:
- Make the mask
- fabricate the channels on the slide
- punch input and output ports

## Design

The design of my chip is very simple. I wanted to do a quick y-channel mix with followed by a serpentine channel and then the outtake. The y-junction combines the two liquids and the serpentine track aids in mixing. This should hopefully be a simple first build.

To make this chip I will be using soft lithography with PDMS as opposed to wet etching or laser ablation. Wet etching on a rigid substrate is much more dangerous and requires stronger chemicals that are overkill for prototyping. Laser ablation requires a very strong and advanced laser that is also beyond my scope at this moment (they typically cost 6 figures!) 

Since this is soft lithography on PDMS, I can punch holes after lithography with just some punches.

## Process for Creating the Chip

1) **Design the mask**
2) **Print the Mask**
3) **Setup UV Soft Lithography**
4) **Bake and Cure? (idk here)**
5) **Add Ports**
6) **Clean and Test!**


### 1) Design the mask

For making the mask, I used onshape to develop the channel 

![[Screenshot 2025-12-24 at 12.21.49 PM.png]]

Then I loaded it into the klayout MEMS software to scale and export the mask file format. In klayout, it looks like this: 

![[Screenshot 2025-12-24 at 12.35.40 PM.png]]

This is a relatively simple design so I don't have to worry about a lot of typical things you need to worry about for the mask design. These issues include worrying about layers and the cell hierarchy for reusable components. 

BTW - klayout is a horribly confusing piece of software at first use. I recommend doing some reading as it took me over a day to fully know how to do some basic operations with it. Although to be fair I could be slow.

 **Ports Note:** Ports do not need to be put in the mask. We can punch these after with a mm punch.

Ok so now that this mask is in klayout. I can export as a gds file! I have put it in the same directory as this chip demo (you won't be able to see it in obsidian but you can check your files.)

### 2) Print the Mask

