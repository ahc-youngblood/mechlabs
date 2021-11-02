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

\collapse{Click to see the answer after you've solved.}{$$ r_\phi = \ell\sin\theta - R\cos\theta $$}

We can plug this into the first equation to find

$$ \dot{\psi} = \left(\frac{\ell}{R}\sin\theta - \cos\theta\right)\Omega $$

Next, we should find the angular velocity. From the diagram we see that

$$ \vec{\omega} = \Omega\hat{e}_z + \dot{\psi}\hat{e}_3 $$

Try breaking $\hat{e}_z$ into its $\hat{e}_1$ and $\hat{e}_3$ components to rewrite $\vec{\omega}$ in terms of those unit vectors.

\collapse{Click to see the answer after you've solved.}{

$$ \hat{e}_z = \sin\theta\hat{e}_1 + \cos\theta\hat{e}_3 $$
$$ \vec{\omega} = \Omega\sin\theta + \Omega\cos\theta\hat{e}_3 + \dot{\psi}\hat{e}_3 $$
}

Now use the expression you got for $\dot{\psi}$ above to get a final form for $\vec{\omega}$

\collapse{Click to see the answer after you've solved.}{
$$ \vec{\omega} = \Omega\sin\theta\left(\hat{e}_1 + \frac{\ell}{R}\hat{e}_3\right) $$

It is not usually the case that the rotational velocity about two principal axes is the same, it leads to some interesting behavior for this system. 
}

To get the angular momentum, should we multiply this angular velocity by a moment of inertia?

\collapse{Answer.}{No. As in class, we have to recognize that there are multiple moments of inertia involved in this case so

$$ \vec{L} = I_1\omega_1\hat{e}_1 + I_3\omega_3\hat{e}_3 $$

We found that $\omega_1$ and $\omega_2$ are the same so

$$ \vec{L} = \Omega\sin\theta\left(I_1\hat{e}_1 + \frac{\ell}{R}I_3\hat{e}_3\right) $$

}

In terms of $\omega_1$ and $\omega_3$, what angle does $\vec{\omega}$ make with the $\hat{e}_3$ vector? What is this in terms of $\ell$ and $R$? Similarly, what angle does $\vec{L}$ make with $\hat{e}_3$? Are $\vec{L}$ and $\vec{\omega}$ in the same direction for this system?

\collapse{Click for the answers when you have thought about this for a while.}{

![Jackson Fig. 2](/assets/jackson_fig2.JPG)
~~~
<p align = "center">
Fig.2 - From Jackson et al., Am. J. Phys., Feb. 2019 
</p>
~~~

$$ \gamma_\omega = \arctan\left(\frac{\omega_1}{\omega_3}\right) = \arctan\left(\frac{R}{\ell}\right) $$

$$ \gamma_L = \arctan\left(\frac{L_1}{L_3}\right) = \arctan\left(\frac{I_1R}{I_3\ell}\right) $$

So they are not in the same direction.
}

$\vec{L}$ precesses as in the case of a tilted top or gyroscope, but its magnitude should not be significantly changed. In our case the angular momentum is given by

$$ \vec{L} = I_3\omega\sin\theta\cos\theta\left[\left(\frac{I_1}{I_3} - \frac{\ell}{R}\tan\theta\right)\hat{r}_{xy} + \left(\frac{I_1}{I_3} -\frac{\ell}{R}\right)\hat{e}_z\right] $$

where $\hat{r}_{xy}$ represents a unit vector in the $x-y$ plane (it is rotatin in this plane at a rate $\Omega$).

## Theoretical Questions

1. What are the expressions for $I_1$ and $I_3$ for (a) a hollow cylinder, (b) a solid cylinder (both of mass $M$, radius $R$, and length $2\ell$? Think about what simple shapes you can combine to get these, no need for integration.

2. Find an expression for the magnitude of $\vec{L}$ if (a) $\theta = \gamma_\omega$ and if (b) $\theta = \gamma_L$. Is there a significant difference between the two?

# Experiment

1. Measure the length and diameter of the hollow pvc cylinder.

2. Set the cylinder spinning using one of the two methods shown in the videos below and record video that includes both the beginning of the spin and the beginning of the roll.
~~~
<iframe width="560" height="315" src="https://www.youtube.com/embed/-s2nt6Tv1cA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
~~~
~~~
<iframe width="560" height="315" src="https://www.youtube.com/embed/j4tGeMJtceI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
~~~

If you use different methods for different trials keep track of which method you used for which trial.

3. Repeat at least three times using the same spinning method/technique.

4. Analyze the video in tracker to find both the initial spin rate $\Omega$ of the cylinder and the linear velocity while rolling after it has finished spinning. Here is a useful guide on extracting rotational velocity in tracker.

~~~
<iframe width="560" height="315" src="https://www.youtube.com/embed/BErYh2n7Y4E" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
~~~

5. Repeat for the solid cylinder (wooden dowel).

## Experimental tips:

* I found that the twist method of starting the cylinder allows for more control of where the cylinder stays but it may be a bit difficult to get started compared to the push method. You may have to try repeatedly before you can get a useable video using any method. Don't give up!

* I found it useful to define three different point masses in tracker:

One for the center of mass, which should be set as the reference frame as shown in the tutorial video and in the image below.

![spinroll set frame](/assets/tracker_center.jpg)

One for a point of the cylinder you track as it goes around the center of mass. This can be difficult. Tracking a point on the edge of the cylinder works well. Tracking a point marked with tape doesn't work as well as you might think -- for interesting reasons -- but give it a try.

One for the cylinder after it has stopped spinning to get the rolling motion separately.

In the end, you should have three tracks looking sort of like the tracks in the images below.

![spinroll track rotation](/assets/tracker_rot.JPG)

![spinroll track rolling](/assets/tracker_roll.JPG)

Autotracker probably only works for the rolling part of the motion.

# Conclusion

1. What were the $\ell/R$ ratios for your solid and hollow cylinders?

2. What were the $I_1$ and $I_3$ moments of inertia for the solid and hollow cylinders?  The masses from my kit are: hollow cylinder (11.4 g), solid cylinder (10.8 g).

3. What were the angles $\gamma_\omega$ and $\gamma_L$ for the solid and hollow cylinders?

4. What maximum rates of spin about the $z$-axis did you find?

5. What were the rotation rates of the cylinder about its main axis while it was rolling?

6. It turns out that $\gamma_\omega$ represents the lower stable value of $\theta$ and $\gamma_L$ represents the upper stable value of $\theta$. Do your observations support conservation of angular momentum through the transition from spinning to rolling for either of these stable tilt angles?

7. Justify your answers to 6. with data analysis.

8. Does the method of starting the cylinder spinning seem to affect which tilt angle is a better choice? Collaborate with your group if you do not have data on both methods of starting.

9. Is kinetic energy conserved across the transition from spinning to rolling? Find the change in kinetic energy. Find a theoretical expression for this change and compare.

~~~
<script>
  var coll = document.getElementsByClassName("collapsible");
  var i;
  
  for (i = 0; i < coll.length; i++) {
    coll[i].addEventListener("click", function() {
      this.classList.toggle("active");
      var content = this.nextElementSibling;
      if (content.style.display == "none") {
        content.style.display = "block";
      } else {
        content.style.display = "none";
      }
    });
  }
</script>
~~~
