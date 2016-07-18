---
ID: 2176
post_title: >
  You Can Solve Quantum Mechanics’
  Classic Particle in a Box Problem With
  Code
author: Staff Writer
post_date: 2016-03-26 00:05:05
post_excerpt: ""
layout: post
permalink: >
  https://www.whenitson.com/you-can-solve-quantum-mechanics-classic-particle-in-a-box-problem-with-code/
published: true
original_cats:
  - >
    numerical calculation,Python,quantum
    mechanics,Science Blogs,Dot
    Physics,Science
original_title:
  - >
    You Can Solve Quantum Mechanics’
    Classic Particle in a Box Problem With
    Code
original_link:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4e83f548/sc/23/l/0L0Swired0N0C20A160C0A30Ccan0Esolve0Equantum0Emechanics0Eclassic0Eparticle0Ebox0Eproblem0Ecode0C/story01.htm
canonical_url:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4e83f548/sc/23/l/0L0Swired0N0C20A160C0A30Ccan0Esolve0Equantum0Emechanics0Eclassic0Eparticle0Ebox0Eproblem0Ecode0C/story01.htm
---
 [ad_1]
<br><div id=""><p>Humans have problems with quantum mechanics. We have excellent intuition about the motion of a tennis ball tossed in the air, but what about an electron trapped in a box? The tendency is to use the same tennis ball rules and apply it to the electron—but it doesn’t work. We have to use different models to explain properties of very very small things. We call this quantum mechanics (as opposed to classical mechanics).</p>
<p>Of course I can’t go over all the details of quantum mechanics, so let me give you the abridged version.</p>
<ul><li>When humans started studying small things, they noticed that classical models didn’t work.</li>
<li>In particular, it seemed clear that electron “orbits” in the hydrogen atom could only exist at certain energies.</li>
<li>In another experiment it was found that shooting electrons through slits would cause interference patterns similar to wave interference.</li>
<li>Why not just say that particles have a wave nature? Why not just adopt some type of wave equation for particles?</li>
</ul><p>OK, it didn’t happen exactly like that—but you get the idea. From these ideas we get the Schrödinger Equation. It’s pretty complicated, so let me start with the simplified version of this equation—the Time Independent Schrödinger Equation. This is probably what you will see when you first start off in quantum mechanics.</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/03/You-Can-Solve-Quantum-Mechanics-Classic-Particle-in-a-Box-Problem-With-Code.jpg" alt="La te xi t 1" width="213" height="72"/></p>
<p>What the heck is this? Let me make some comments.</p>
<ul><li>This is the one dimensional TISE in which the variable is just x.</li>
<li>ψ is called the wave function. It’s the part that’s “waving” when we consider the wave properties of matter. But just like the the intensity of light is proportional to square of the electric field, the observable stuff depends on |ψ|<sup>2</sup>.</li>
<li>|ψ|<sup>2</sup> gives you the probability density—this lets you determine the likely locations of the particle. In quantum mechanics, we don’t deal with equations of motion, we deal with probability.</li>
<li>E is the energy of the particle and V is the potential energy of the system. Yes, it’s weird that we use V for potential energy instead of U (normally V is the electric potential). I have no idea why.</li>
<li>ℏ is a constant and m is the mass of the particle.</li>
</ul><p>That’s your quick intro to quantum mechanics.</p>
<h3>Particle in a Box</h3>
<p>The very first problem you will solve in quantum mechanics is a particle in a box. Suppose there is a one dimensional box with super stiff walls. There is a ball in that box that can bounce back and forth with no energy loss.</p>
<p>How do you use the TISE to find the wave function for this case? Well, we already have a differential equation—but a solution for ψ also must satisfy the following conditions.</p>
<ul><li>It must be continuous.</li>
<li>ψ must be zero in regions where the particle can not be found (like outside the box).</li>
<li>As x goes to +/- infinity, ψ must go to zero.</li>
<li>ψ must be normalizable. This means that you have to be able to integrate |ψ|<sup>2</sup> over all of x and set it equal to one. This is the same as saying the probability of finding the particle <em>somewhere</em> is 1 out of 1.</li>
</ul><p>We just need one more thing—an expression for the potential energy. If we have a box with walls at x = 0 and x = L, then the potential will be zero from x = 0 to L and infinite everywhere else. Now it’s just a matter of solving the differential equation and apply the conditions above.</p>
<p>I’m going to skip this part because I really want to get to a numerical solution. You should work through this yourself, it’s also probably in your physics textbook. However, this is the solution for the wave function inside the box (outside it’s zero).</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/03/1458950705_223_You-Can-Solve-Quantum-Mechanics-Classic-Particle-in-a-Box-Problem-With-Code.jpg" alt="La te xi t 1" width="207" height="113"/></p>
<p>For the wave function,<em> A</em> is just some constant (you can find this through normalization) and <em>n</em> is an integer number. Since you have a sinusoidal solution for the wave function with a boundary condition, multiple values of <em>n</em> will work. With integer values of <em>n</em>, we also get the quantized energy values as shown above.</p>
<p>In 1926 Schrödinger published a paper describing his ideas. The title of the paper was “Wave Mechanics”—not Quantum Mechanics. This is important as it is the wave nature of matter that leads to quantized energies. I just like to point that out.</p>
<h3>Numerical Solution for a Particle in a Box</h3>
<p>The analytic solution to the infinite square well is nothing new. You can find this in every intro quantum mechanics textbook. But how can we solve it numerically? Just to be clear, by “numerically” I mean the process of breaking a problem into many smaller problems (<a href="http://www.wired.com/tag/numerical">you can see many examples here</a>).</p>
<p>The Schrödinger equation is a differential equation. It makes a connection between the second derivative of<span>ψ</span> (d<sup>2</sup>ψ/dx<sup>2</sup>) and ψ. We can use the same idea to find the updated position of a particle with a force to find the numerical values of the wave function. Recall this basic strategy from a numerical calculation in classical mechanics (where <em>p</em> is the momentum):</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/03/1458950705_615_You-Can-Solve-Quantum-Mechanics-Classic-Particle-in-a-Box-Problem-With-Code.jpg" alt="La te xi t 1" width="179" height="115"/></p>
<p>I can do the same thing with the wave function. Let me use dot-notation to represent the derivative (ψ-dot is the first derivative and ψ-double dot is the second). This gives the following approximation (technically, I am using the dot-notion incorrectly but let’s just do it anyway).</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/03/1458950705_825_You-Can-Solve-Quantum-Mechanics-Classic-Particle-in-a-Box-Problem-With-Code.jpg" alt="La te xi t 1" width="170" height="111"/></p>
<p>Notice that I am using ψ-dot<sub>2</sub> to calculate the new value of ψ. This is of course wrong in that I should actually use the average ψ-dot. However, this will still work if Δx is small. Now I have the following recipe:</p>
<ul><li>Start at x = 0 m and ψ = 0 (also I will pick ψ-dot equal to zero).</li>
<li>Use Schrödinger’s equation to calculate ψ-double dot.</li>
<li>Use ψ-double dot to calculate ψ-dot.</li>
<li>Use ψ-dot to calculate ψ.</li>
<li>Update the x-position and do it again until you get to the end of the box.</li>
</ul><p>But wait! What about the energy (E) in the Schrödinger equation? For now, just guess a value for the energy. Let’s start with E = 0. Just push the “play” button to run the code.</p>

<p>Clearly an energy of zero doesn’t work since the wave function isn’t zero at x = L. Maybe we should try a different energy. Just pick something (I suggest a value from 1 – 10). Go ahead and change the code (click the pencil icon to edit if you don’t see the code) and then run it again. You can see that as you increase the energy above 0, the wave function gets closer and closer to zero at x = L. Of course you could just keep guessing until you find a solution, or we could make the computer do it.</p>
<p>Here is a different program that finds the energy for which ψ = 0 at x = L. It’s called the <a href="http://wwwitp.physik.tu-berlin.de/brandes/public_html/qm/qv3.pdf">“shooting method”</a> since we calculate ψ again and again until we get the right answer. It’s sort of like shooting a ball at a target and changing the launch angle and reshooting until we hit the target.</p>
<p>Let’s look at the code and then I will point out some parts of it.</p>

<p>A few notes on different lines in the code (by line number):</p>
<ul><li><strong>11.</strong> I start off with E = 0, but I am going to increase this value. dE is the amount I increase in each re-run. You could change this to a smaller value if you want a more accurate solution.</li>
<li><strong>12.</strong> I am making a boolean variable called “searching”. When I find a value for the energy that works, I will no longer be searching so searching will be set to False.</li>
<li><strong>13.</strong> This is the loop that searches for the best energy.</li>
<li><strong>14.</strong> rate(1000) says to not do more than 1000 loops per second so that you can see how the thing changes.</li>
<li><strong>15 – 18.</strong> I need to reset the variables before solving the differential equation. f1.delete() clears the previous graph.</li>
<li><strong>19.</strong> This is the same loop as in the previous program in which the solution to Schrödinger equation is solved.</li>
<li><strong>29.</strong> Here I check if the final value of ψ is close to zero.</li>
</ul><p>That’s it. When you run this you can see that an energy of 4.92 gives a fairly nice solution to this infinite square well. But wait! There’s more! Go back to the code and change the starting energy (in line 10) to 5 instead of zero. Now the shooting method won’t find the energy level that it did before since it only searches “up.” Go ahead and run the code with this new starting energy and you can find the next energy level that works.</p>
<h3>Normalization of the Wave Function</h3>
<p>I said we were finished, but clearly that was a lie. I don’t have the correct wave function. There is one more condition that must be satisfied. Since the square of ψ (technically the complex conjugate) is the probability density, the integral of this over all space must be 1. In other words, the total probability of finding the <em>anywhere</em> must be 1.</p>
<p>OK, let’s start off by comparing our numerical wave function to the analytical solution. If you normalize this analytical function, you will find the following solution.</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/03/1458950705_838_You-Can-Solve-Quantum-Mechanics-Classic-Particle-in-a-Box-Problem-With-Code.jpg" alt="La te xi t 1" width="208" height="121"/></p>
<p>Instead of just plotting the probability density for both solutions, I will also integrate to find the total probability. Since I am dealing with a numerical solution, the integration is fairly simple. I have the values of |ψ|<sup>2</sup> at different values of x. The next value is just at x + dx. So, imagine a rectangle that has a length of |ψ|<sup>2</sup>*dx. All I need to do is to go through each value for |ψ|<sup>2</sup>, calculate the area of this tiny rectangle and add it to the total area. Here is what I get.</p>

<p>Notice that the red curve shows the probability density for the textbook solution (the analytical solution) and the blue is the numerical. The numerical solution has a total probability of 0.0508895. Clearly we need to change the numerical solution so that the total probability is 1. There are a couple of ways to change fix this—let’s try changing the initial derivative of ψ. Recall that I arbitrarily set this equal to a value of 1 for the initial conditions. What if I increase this to 2? Go ahead and try that by changing the value in the code above (in line 8). Now re run the program and you should get a numerical probability of 0.203558. That’s closer to 1, but still not correct. OK, here is the trick (and it will lead to a homework question). What if you set the initial ψ derivative to 1/sqrt(0.0508895)? Go ahead and try that. <em>Boom</em>. You just normalized the wave function.</p>
<h3>Homework</h3>
<p>Is this going to be on the test? Yes, it is now. Here are some questions for you.</p>
<ul><li>Find the first 10 energy levels in the numerical calculation. Show that E<sub>n</sub> is proportional to n<sup>2</sup>.</li>
<li>Can you find a better method for calculating the wave function? Try searching for another method and creating it in python (or whatever language you like).</li>
<li>How could you make this calculation faster? In my code, the energy steps are always the same. Is it possible to use some non-constant energy jumps to find the correct energy?</li>
<li>Why does the initial derivative of ψ set the normalization? Start with the analytical solution for ψ and show that at x = 0, the derivative gives 1 over the squareroot of the total probability.</li>
<li>What if you don’t have a flat infinite potential well? What if one side is raised by some energy (just pick something). How would this change your solution? Go ahead and try this.</li>
<li>Use the numerical calculation above to find the probability of finding the particle between x = 0 and x = L/5.</li>
</ul><a class="visually-hidden skip-to-text-link focusable bg-white" href="#start-of-content">Go Back to Top. Skip To: Start of Article.</a>

			
</div>
<br>[ad_2]
<br><a href="http://feeds.wired.com/c/35185/f/661370/s/4e83f548/sc/23/l/0L0Swired0N0C20A160C0A30Ccan0Esolve0Equantum0Emechanics0Eclassic0Eparticle0Ebox0Eproblem0Ecode0C/story01.htm">Source </a>