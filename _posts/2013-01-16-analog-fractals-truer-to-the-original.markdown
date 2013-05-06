---
layout: post
title: ! 'Analog Fractals: Truer to the Original'
category: posts
---

This post is all about how to draw fractal curves by hand, like these!

![Analog Fractals][all]

---

In high school one of my friends showed me how to draw the <a href="http://en.wikipedia.org/wiki/Dragon_Fractal">Heighway Dragon Curve</a> by hand. Ever since then, most of my drawings end up looking  like one of these fractals above. There's  plenty of algorithms  for making  these  fractals on a computer. However, unless you, the reader, are actually a data-mining program sifting through this post for  information, then you'll need a different algorithm to draw these efficiently.

After this, your doodles will never be the same.

Equipment:
<ol>
	<li><span style="line-height:13px;">Graph Paper (the smaller, the better)</span></li>
	<li>Your favorite writing utensil (pencil is good for learning, pen is great for showboating)</li>
</ol>
##The Tree Fractal (Difficulty: EZPZ)

![Tree Fractal][smalltree]

This fractal looks like a tree.  A really awesome tree. It's a derivative of  the <a href="http://en.wikipedia.org/wiki/Pythagoras_tree_(fractal)">Pythagoras Tree  Fractal</a>. Let's do this!

![Tree Fractal Instructions][treeInstr]

1. Start with a line on a piece of graph paper. Make the line a length of some integer power  of 2 (1, 2, 4, 8, 16...) for best results.

2. The top point of that  line is where the  tree is going to "grow" (I marked the growth points with red).  Draw 2 lines forking off of the original line at 45 degree  angles that pass through half  as many squares as the first  line.  For example, if you started with a line 4 squares long, then the branches should  pass through 2 squares diagonally.

3. The  top points of the two new lines are where the tree will grow again. This time draw one line upwards along the grid line and one pointing away from the center  of the tree. They pass through as many squares on the grid as the previous branch, only these new branches will be shorter since they go along the edge of the square instead of the diagonal.

4. Each of these new lines is the start of a new tree.  Repeat until you can't draw new lines because they're too small to fit nicely on the graph paper.

Q: What if  the branches collide!?

A: Overlap on the branches is what makes this look even more like a tree. Keep following the same rules and then something like this happens:

![Big Tree Fractal!][16tree]

Warning: This is an  O(2^n) algorithm. Colloquially, it's "wicked slow". A bigger starting length means that  you'll get a cooler looking tree, but the number of lines you need to draw and thus time it takes grows very quickly. Worth it? Sometimes, it really depends on your situation.

##The Lévy C Curve (Difficulty: Harder than the tree)

![The Levy C Curve][levy]

The <a href="http://en.wikipedia.org/wiki/L%C3%A9vy_C_curve">Lévy C Curve</a> is a pretty sweet fractal.  This one is closely related to the dragon fractal, but is much easier to draw. Ready? Great.

![Levy Curve Instructions][LevyInstr]

1. Start with two lines forming coming together to form a right angle. I made them 2 squares long, but I highly suggest you use lines that are only one square long on your graph paper. The red dotted line indicates an axis of rotation we'll use to 'flip' the fractal to create the next iteration. To illustrate the  'flip' with your hand, place your hand on a flat surface palm up. Then, keeping your little finger on the surface, twist your wrist so that your hand flips over on  the surface, palm down. That's what we're going to do with the curve on the page.

2. The red axis is like a mirror.  By drawing the piece we started with's 'reflection' we get the next iteration. You can also imagine this step as swinging a copy of what we already drew around the axis and putting it back on the page. Our new axis of rotation is going to be 45 degrees off of the original, as indicated in the drawing.

3. To make the figure in 3, we rotated everything we had in part 2 around that 45 degree axis. The 45 degree rotation axis always starts at the end of the Lévy curve line.

4. Continue the process of flipping across the axis of rotation, alternating between the original axis and the 45 degree off axis. Eventually you'll run out of room on the paper and the curve will look awesome!

##The Dragon Fractal (Difficulty: Actually takes some practice)

![Dragon Fractal][dragon]

This looks familiar yes? If you read Jurassic Park it should.  In the novel, this beautiful fractal is used to represent the park's descent into chaos.  Also known as the <a href="http://en.wikipedia.org/wiki/Dragon_Fractal">Heighway Dragon</a>, it  is simply beautiful.

![Dragon Instructions][dragonInstr]

1. Start with a straight line.  On my page, it's two units long, but using a one unit long line means you'll have more space to grow this beast. The red dot marks the anchor point for this iteration of the fractal. While we made the Lévy C Curve by reflecting a copy of the image across an axis, the dragon fractal is constructed by rotating a copy of the image about the anchor point.

2. To make the image in step 2, imagine lifting up a copy of the line in step 1, rotating it 90 degrees to the left about the anchor point, then placing it back down on the page. The end point of the new line, marked in red, is the new anchor point. The previous anchor point is marked in blue to help you visualize the rotation process.

3. For the image in step 3, rotate the ENTIRE image in part two about the anchor point 90 degrees to the left. This is the rule for growing the fractal. Since we started with rotating to the left, we must rotate it to the left every time.  You could also start by rotating to the right, then rotating it to the right every time.

4. Like each of the other steps, this is made by rotating the ENTIRE figure about the anchor point. Notice that the hook shape from step 3 is rotated to make the image in step 4. Repeat this rotation process until you're out of room (or can't draw the next step without getting hopelessly lost).

###Extra Tips For the Dragon Fractal:

A good sort of training wheels way to build the dragon fractal (especially as it gets larger) is to draw two copies of it, one on it's own sheet of paper.  You then have one copy to physically rotate to see what the next piece actually looks like without having to imagine it in your mind.

On the dragon, error checking can get quite difficult as the fractal grows since it doesn't have a symmetric shape like the tree and the C curve. It helps a lot to cheat and look at pictures of what the curve is supposed to look like at a given iteration.

<a href="http://en.wikipedia.org/wiki/Fractals">Fractals!</a>

---

[all]: /images/analog-fractals/fractals2.jpeg "Fractals!"
[dragon]: /images/analog-fractals/dragon.jpeg "RAWRRR!"
[dragonInstr]: /images/analog-fractals/dragonInstr.jpeg
[Levy]: /images/analog-fractals/levy.jpeg
[levyInstr]: /images/analog-fractals/LevyInstr.jpeg 
[16tree]: /images/analog-fractals/16Tree.jpg
[treeInstr]: /images/analog-fractals/treeInstr.jpeg
[smallTree]: /images/analog-fractals/smallTree.jpeg
