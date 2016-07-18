---
ID: 542
post_title: >
  Use Code to Create Sweet 3-D
  Visualizations of Electric Fields
author: Staff Writer
post_date: 2016-01-29 18:33:42
post_excerpt: ""
layout: post
permalink: >
  https://www.whenitson.com/use-code-to-create-sweet-3-d-visualizations-of-electric-fields/
published: true
original_cats:
  - >
    electric field,Python,vpython,Science
    Blogs,glowscript,Dot Physics,Science
original_title:
  - >
    Use Code to Create Sweet 3-D
    Visualizations of Electric Fields
original_link:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4d3a84be/sc/28/l/0L0Swired0N0C20A160C0A10Cuse0Ecode0Eto0Ecreate0Esweet0E30Ed0Evisualizations0Eof0Eelectric0Efields0C/story01.htm
canonical_url:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4d3a84be/sc/28/l/0L0Swired0N0C20A160C0A10Cuse0Ecode0Eto0Ecreate0Esweet0E30Ed0Evisualizations0Eof0Eelectric0Efields0C/story01.htm
dsq_thread_id:
  - "4537453907"
---
 [ad_1]
<br><div id=""><p>I’ve already made the argument that <a href="http://www.wired.com/2015/08/coding-physics-course/">numerical models (using computer code) should be an integral part of the introductory physics course</a>. But what if you don’t know where to start? Suppose you are either in or teaching the second semester of introductory physics. What do you need to get started? I’m here to help you with that.</p>
<p>First, a couple of notes about numerical calculations with <a href="http://www.vpython.org">VPython</a>.</p>
<ul><li>First, there is <a href="http://www.vpython.org">VPython</a>. This is a visual module for python that makes it relatively simple to create 3-D objects. Oh, and it’s still python. However, if you don’t have python installed on your computer—you might need to do a little bit of work. This is fine if you plan on doing lots of stuff (and using other modules) but maybe not so great for students.</li>
<li>Next, there is <a href="http://www.glowscript.org">GlowScript</a>. In short, this is VPython in a web browser based on <a href="http://rapydscript.pyjeon.com/">RapydScript</a> (a JavaScript Python-to-JavaScript compiler that makes this possible). GlowScript is the platform that I recommend for students. They don’t need to install anything and it’s easy to switch to a different computer since stuff is saved online. Oh, GlowScript code runs on my phone too.</li>
<li>Finally, there is <a href="http://trinket.io">trinket.io</a>. This is like GlowScript in that it is VPython running in your browser. However, this is one big difference—you can embed trinket code into a webpage. This makes it great for instructional uses. Also, you can either show the code or just show the running program. Students can edit the code without having to login in. It’s really nice.</li>
</ul><h3>Electric Field Due to a Point Charge</h3>
<p>Now for some physics. Let’s start with the electric field due to a point charge. If I have some charge, <em>q</em> then the electric field will be pointed radially outward (for a positive charge) and decrease in strength as you get farther away from the charge. This can be written as the vector equation:</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/01/Use-Code-to-Create-Sweet-3-D-Visualizations-of-Electric-Fields.jpg" alt="La te xi t 1" width="246" height="128"/></p>
<p>Let’s just jump right into a calculation. Suppose I have a 3 nC charge at the location &lt;0.1, -0.2, 0&gt; m. What is the electric field at a location &lt;-0.4, 0.2, 0.1&gt; m? Normally, I would make a sketch to show you what’s going on. However, in this case I am going to make a program. Here is what this looks like. The red sphere is the charge and the small white sphere is the location of the calculated electric field.</p>

<p>Although I added comments in the code, let me add some notes along with some things you should try.</p>
<ul><li>This stuff is in 3-D. If you right click with the mouse you can rotate things around.</li>
<li>There are two types of 3-D objects used in this code. There is the sphere and the arrow. These have different properties, but if you play with it a bit you can probably grok them.</li>
<li>I have to add a scale factor in front of the electric field. In fact, you can change that value and see what happens. I encourage you to try that.</li>
<li>This code will calculate E no matter where the charge and observation location are. In fact you can use this little code to check your homework. Just change the values for q, charge.pos, and obs.pos.</li>
<li>Finally, you can print out the values at the end.</li>
</ul><p>If you don’t understand any part of the code—change it. Don’t worry, you can’t really mess anything up. If you change the code and can’t get it back to working order just reset it.</p>
<h3>Electric Field Due to Two Point Charges</h3>
<p>Let’s do another example. Here I want to do something very similar to the problem above. In fact, let’s use the same charge at the same location with the same observation location. However, I want to add a second electric charge with a value of of 2 nC at a location of &lt;0.2, 0.1, 0&gt; m.</p>
<p>Here is the output of the code that calculates the total electric field. Notice that I am no longer displaying the position vectors—I don’t think those are necessary.</p>

<p>Now it is your turn to make this same calculation. Here is some starting code. It doesn’t work right now, but if you add some stuff you should be able to get it to make the same output as above.</p>

<p>Remember, you can’t break anything. If you get stuck, go back to the program with just one point charge. Once you get it working with the same values as my example, you can try changing the location of point charges or the location of the observation.</p>
<h3>Electric Field Due to a Dipole</h3>
<p>A dipole is just two electric charges (of value +<em>q</em> and –<em>q</em>) separated by some distance (<em>s</em>). So, the net charge on a dipole is zero Coulombs but since the two charges are separated there is still an electric field created by the pair. It turns out that these electric dipoles pop up in lots of cases (or at least many things can be approximated as a dipole).</p>
<p>When you have two electric charges, you can find the total electric field at some point in the normal manner of adding the contributions due to the two charges. However, we can also find an approximate value for the magnitude of the electric field due to a dipole as long as we are looking at the field along the axis of the dipole or perpendicular to the axis.</p>
<p>I will leave the derivations of these to you (<a href="https://www.youtube.com/watch?v=h0wjy5qXtxc">or you can watch this video</a>). But here are expressions for the field perpendicular and parallel to the axis of the dipole.</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/01/1454092422_210_Use-Code-to-Create-Sweet-3-D-Visualizations-of-Electric-Fields.jpg" alt="La te xi t 1" width="242" height="128"/></p>
<p>In these equations, <em>r</em> is the distance from the center of the dipole to the point where you want to find the electric field. Also, this is just an approximation for the case where <em>r</em> is much greater than <em>s</em>.</p>
<p>Enough about dipoles. Let’s calculate the electric field due to a dipole. Check out this program.</p>

<p>Now you can play with the code. Here are some things to try.</p>
<ul><li>What happens when you move the observation location to some other place? Try changing the value of obs.pos.</li>
<li>What about the case for the magnitude of the electric field along the axis of the dipole? In this orientation, that would have to be an observation location with just <em>x</em> values and <em>y</em> and <em>z</em> values of zero. Does the calculation agree with the approximate formula? How far along the x-axis do you have to move to get an agreement?</li>
<li>Do the same thing for the electric field perpendicular to the axis of the dipole—this would be an observation location along the y-axis.</li>
<li>Here is the cool part. Make a plot of the calculated magnitude of the electric field along the x-axis as a function of <em>x</em> (which would also be <em>r</em> in this case). On the same plot include the approximation value of the electric field. Note: there is a way to do this in python, but if you aren’t sure how to do that just change the value of obs.pos and record the magnitude of the electric field. Repeat until you have enough data to use whatever plotting method you like best.</li>
</ul><p>That’s it. You have now used python to calculate electric fields. This is just the first step to doing some really cool stuff.</p>

			<a class="visually-hidden skip-to-text-link focusable bg-white" href="#start-of-content">Go Back to Top. Skip To: Start of Article.</a>

			
</div>
<br>[ad_2]
<br><a href="http://feeds.wired.com/c/35185/f/661370/s/4d3a84be/sc/28/l/0L0Swired0N0C20A160C0A10Cuse0Ecode0Eto0Ecreate0Esweet0E30Ed0Evisualizations0Eof0Eelectric0Efields0C/story01.htm">Source </a>