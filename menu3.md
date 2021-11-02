@def title="Angular Momentum Conservation:Spinning and Rolling"

# Items from Lab Kit Needed:

Piece of PVC Tube (Hollow Cylinder)\\
Piece of Wooden Dowel (Solid Cylinder)\\
Brightly Colored Tape\\ 
Ruler\\

~~~
<iframe width="560" height="315" src="https://www.youtube.com/embed/2-3SgJaXfRM" title="YouTube video player" frameborder="0" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
~~~

In this lab, you will study some aspects of the motion shown the video above. In particular, we are interested in whether angular momentum and rotational kinetic energy are conserved through the transition from spinning and rolling to just rolling.


# Theory

![Rolling Objects](/assets/objects_A_small.jpg)

![Jackson Fig. 1](/assets/jackson_fig1.JPG)
~~~
<p align = "center">
Fig.1 - From Jackson et al., Am. J. Phys., Feb. 2019 
</p>
~~~

When a cylindrical object is spun as shown in the video, it actually also rolls without slipping on one edge. The figure above depicts a side view of this situation. Its motion has a lot of similarities to the precessing top discussed in lecture so please bear that in mind.

The important parameters are:
* $ R $: radius of cylinder
* $ \ell $: *half* of the length of the cylinder
* $ \tilde{\ell} = \ell/R $: equal to length of the cylinder divided by 2$R$.
* $ \Omega $: rate of rotation (angular velocity) about $z$-axis.
* $ \dot{\psi} $: rate of rotation about the cylinder's main principal axis.
* $ \hat{e}_z $: Unit vector in the $z$ direction. Same as $\hat{k}$.
* $ \hat{e}_1 $: Unit vector in the plane of the cylinder's perpendicular principal axis.
* $ \hat{e}_3 $: Unit vector in the direction of the cylinder's main principal axis (along its length).
* $ r_\phi $: The part of the cylinder half-length $\ell$ that is parallel to the ground.
* $ \theta $: The angle that the cylinder makes with the vertical (measures how tipped over it is).

Since the edge of the cylinder traces out a circle of radius $r_\phi$ on the ground while rolling about about its axis, we get

$$ r_\phi\Omega = R\dot{\psi} $$

Now, we need to determine $ r_\phi $. Look at the diagram and try to determine what $ r_\phi $ would be in terms of $ R,\ell $, and $ \theta $. 

\collapse{Click to see the answer after you've solved.}{

$$ r_\phi = \ell\sin\theta - R\cos\theta $$

}


### Instruction 1.
* The masses from my kit are: hollow cylinder (11.4 g), solid sphere (66.7 g), solid cylinder (10.8 g). If you have them available, you should use the values from your kit because they will more closely match the motion you record.

### Instruction 3.
* You may find it difficult to do 3b. until later this week, but ask me about it now if you like.

### Instruction 4.
* To keep the ball bearing rolling straight, you will probably have to use the aluminum track. Make sure to place this track on the wooden board to keep it stable and avoid bending/damaging it..
* The hollow cylinder may be especially difficult to track in your video (see below), think about what point would be best to select or if you can use a different camera angle.

![Rolling Cylinder](/assets/cylinder_rolling_frozen.jpg)

### Instruction 6.
* The board does not have enough room to carry out a head-to-head race, so we will have to settle for records.
* To simulate a race, make a video for each object starting from the same height on a ramps with the same incline angle and compare the time taken to reach the bottom.

## p.108

* You will have to use the File>Export>Data File... feature of tracker to extract the v vs. t data and get a trendline in Excel or Google Sheets.
* You do not need to make any animations or animated slides.

[Online Version of Motion Tracking software](https://tracker.physlets.org/trackerJS/)

~~~
<script>
  var coll = document.getElementsByClassName("collapsible");
  var i;
  
  for (i = 0; i < coll.length; i++) {
    coll[i].addEventListener("click", function() {
      this.classList.toggle("active");
      var content = this.nextElementSibling;
      if (content.style.display === "block") {
        content.style.display = "none";
      } else {
        content.style.display = "block";
      }
    });
  }
</script>
~~~
