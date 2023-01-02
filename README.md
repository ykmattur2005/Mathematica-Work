# Mathematica-Work
Yashas Mattur - Modeling Projects in Mathematica

Here's my crazy "work of art"! In creating this, I was inspired by the characteristic double-helix shape of a strand of DNA, so I decided to recreate it using the techniques for graphing 3D lines, curves, and tubes that I had learned in this Try It.

The first step of this process is to create the "backbone" of the DNA, which is shaped like a double helix. To do this, I first started with defining the parametric equation of a regular helix, which is {cos(t), sin(t), t}. Here, the t value ranges from -2Pi to 2Pi; I'm using a pretty large range to make sure my DNA is long enough to see several curls. Then, to create my first helix (which I called "helixA", I created a curling tube made of circles centered on this helix curve, with a radius of 0.25 and oriented parallel to the xy plane. To create my second helix, "helixB", I did the same thing as the first helix, except I centered my circle at {-cos(t), -sin(t), t}. This made it so that the second helix was placed opposite to the first, so that when they're together, it appears as if they intertwined.

Next, I wanted to create the "ladder" part of the DNA - the thin lines of molecules that hold the two helices together. In fact, in a real DNA molecule, this part encodes the A, T, G, and C molecules that encode genetic information, and I'm representing this part with red lines. To draw this, I first created an empty list (called "lines") that I would fill up with parametric plots of lines. Next, I used a for-loop to generate 17 red parametrized lines and insert each one into the list "lines"; this for-loop starts at a = -2Pi and goes up Pi/4 each iteration of the loop until it stops at a = 2Pi; and for every one of those seventeen numbers, the parametric line {tcos(a), tsin(a), a} generates a slightly higher line that's slightly twisted, so that both ends of every line are connected to two opposing helices. Furthermore, the t value here always ranges from -1 to 1, because the helices are always exactly the same short distance from each other. I made all of these lines red with a thickness of 0.05, so that they're clearly visible.

Finally, I plotted this all on the 3D Plotter. I made the length of the axes 0 so that they don't interfere with the visibility of my DNA model.

I hope you like this small model!
