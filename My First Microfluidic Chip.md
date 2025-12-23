by Blake!

In this demo I'll be designing and fabricating my first microfluidic chip. 

## Process for Creating the Chip

1) Make the mask
2) ...


### 1) Make the mask

For making the mask, I used onshape to develop a basic centerline and export the dxf of this line and then I used klayout to generate the mask. Here is the centerline! [[Screenshot 2025-12-22 at 5.24.48 PM.png]]

and here is the dxf loaded into klayout!! [[Screenshot 2025-12-22 at 5.25.16 PM.png]]

KLayout is a very confusing piece of software so I took some time to explore how to use it and I encourage you to as well. The first hiccup I ran into was viewer vs editor mode (this is important since klayout auto loads the viewer which means you can't change anything!).

Now in klayout, how did I make the mask? Well, first thing to notice is the centerline template is a line and not an area. The second thing I did was realize I messed up. Apparently there is no clean way in klayout to create an area from this line (chatgpt lied to me I swear I'm not dumb.). So I resorted to using the python api for klayout. 

I wrote a quick python script to take this python path and turn it into an area