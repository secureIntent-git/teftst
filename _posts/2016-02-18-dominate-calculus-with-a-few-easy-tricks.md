---
ID: 1112
post_title: Dominate Calculus With a Few Easy Tricks
author: Staff Writer
post_date: 2016-02-18 22:55:04
post_excerpt: ""
layout: post
permalink: >
  https://www.whenitson.com/dominate-calculus-with-a-few-easy-tricks/
published: true
original_cats:
  - >
    Python,Science Blogs,numerical,math,Dot
    Physics,calculus,Science
original_title:
  - Dominate Calculus With a Few Easy Tricks
original_link:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4db0c8f3/sc/27/l/0L0Swired0N0C20A160C0A20Cdominate0Ecalculus0Ewith0Ea0Efew0Eeasy0Etricks0C/story01.htm
canonical_url:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4db0c8f3/sc/27/l/0L0Swired0N0C20A160C0A20Cdominate0Ecalculus0Ewith0Ea0Efew0Eeasy0Etricks0C/story01.htm
---
 [ad_1]
<br><div id=""><div id="small-art" data-share="">
				<figure attachment_1975773="" class="carve wp-caption square alignnone  relative" data-js=""><a href="http://www.wired.com/wp-content/uploads/2016/02/numerical-integration-computer-integrals-500149643.jpg"><img class="size-default-top-art wp-image-1975773" data-pin-description="Dominate Calculus With a Few Easy Tricks" src="http://www.whenitson.com/wp-content/uploads/2016/02/Dominate-Calculus-With-a-Few-Easy-Tricks.jpg" alt="500149643" width="582" height="582"/></a><figcaption class="wp-caption-text link-underline"><span class="credit link-underline-sm"><span aria-hidden="true" class="ui ui-illo inline-block ui-credit relative opacity-5 marg-r-micro"/> Getty Images</span></figcaption></figure></div>

			<p>How do you integrate with a computer? Let’s start with an example.</p>
<p>Suppose a car travels only in the x-direction. It starts at x = 0 m with a velocity of 0 m/s. If the car has a constant acceleration of a (let’s pick 1.5 m/s<sup>2</sup>), how far will it travel after four seconds? You should be able to solve this problem in a number of ways. You could start with the definition of acceleration and integrate twice or you could use the kinematic equations. I’m not going to go over either of these solutions since they aren’t very interesting.</p>
<p>How would you solve this numerically (when I say “numerical,” others might say “computational”)? The key to just about every numerical solution is to break a complicated problem down into a bunch of simpler problems. But what’s simpler than a constant acceleration problem? A constant velocity problem. Yes, let’s do that. If an object moves with a velocity <em>v</em>, how far does it travel during some time interval? Let’s start with the definition of velocity (in one dimension):</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/02/1455836104_614_Dominate-Calculus-With-a-Few-Easy-Tricks.jpg" alt="La te xi t 1" width="141" height="107"/></p>
<p>But what if I represent this as a graph? Here is a velocity vs time graph for this same situation.</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/02/1455836104_985_Dominate-Calculus-With-a-Few-Easy-Tricks.jpg" alt="Spring 2016 Sketches key" width="298" height="199"/></p>
<p>As you can see from this plot, the distance traveled would be equivalent to the area under the velocity-time graph. OK, so what if the velocity is changing? What about the case of a constant acceleration? We can still find the displacement as the area under the curve by using a similar method. Let’s just break the curve into many small rectangles where we assume the velocity is constant.</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/02/1455836104_874_Dominate-Calculus-With-a-Few-Easy-Tricks.jpg" alt="Spring 2016 Sketches key" width="276" height="194"/></p>
<p>Here I am calling the width of this rectangle <em>dt</em> instead of Δt to emphasize that it is a very small time interval. The other big difference is that the velocity is not constant and it also changes with time. But note that I have a strategy for calculating the displacement (which is the same as integrating).</p>
<ul><li>Start with initial values for position, velocity, and time.</li>
<li>Pick a tiny time interval (dt).</li>
<li>Calculate the area of this tiny rectangle with width dt and add this to the total area.</li>
<li>Increase the time value by dt.</li>
<li>Use this new time to calculate the new velocity.</li>
<li>Repeat.</li>
</ul><p>Let’s do this with some python. One important note: If you don’t have exact values, you can’t get an answer. You have to use numbers. Also, this only gives a numerical answer and not a function (we can fix that later). I will also include an analytic solution so that we can compare results.</p>

<p>You can see the two values for the displacement. With a fairly large time interval of 0.1 seconds, I still get a displacement fairly close to the analytical solution of 12 meters. Making a smaller time interval will clearly give a better solution. Also, some might complain that my method sucks. I am using the velocity at the beginning of the interval instead of at the end or the middle. Yes, you can debate which velocity would be best, but this is a beginner’s guide to numerical integration. Hopefully these differences won’t matter as my time interval gets small.</p>
<p>But this isn’t what you wanted—I know. You want a function that represents this integral. I can do that, but let me first write out analytically what you are looking for.</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/02/1455836104_45_Dominate-Calculus-With-a-Few-Easy-Tricks.jpg" alt="La te xi t 1" width="172" height="64"/></p>
<p>You want the solution for <i>all</i> values of <em>t</em>. To get this I can find the displacement for <em>t</em> = 0.1 s, then 0.2 s, and then 0.3 s and so on. That means doing the same numerical integration above a bunch of times. The easiest way to do that is with a python function. I’m not going to go over all the details of a function, but <a href="https://phys221.wordpress.com/2015/03/09/glowscript-tutorial-6-functions/">here is a quick tutorial</a>.</p>
<p>Hopefully this code will make at least a little bit of sense. I plot both the analytical and numerical solutions.</p>

<p>There you go. That’s the function you were looking for—and it seems to work just fine.</p>
<p>Now how about a complicated case? The integration problems that always caused me problems were ones that involved trig substitution. How an integral that uses both trig sub and integration by parts? Here is the integral we will solve.</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/02/1455836104_963_Dominate-Calculus-With-a-Few-Easy-Tricks.jpg" alt="La te xi t 1" width="220" height="76"/></p>
<p>I did something wrong here, because I am lazy. I shouldn’t have the integration variable the same as the function variable. Really, inside the integral it should say “<em>x</em>‘”, but that would look weird. OK, I’m sorry.</p>
<p>Let me just jump right into the numerical solution. I can also plot the analytical solution by <a href="http://tutorial.math.lamar.edu/Classes/CalcII/TrigSubstitutions.aspx">following the answer from this page</a>. Oh, one note. I am going to call the stuff inside the integral <em>g(x)</em> just to make the calculation easier.</p>

<p>Notice that I used the analytic solution from that same website so you can see the two plots are nearly identical. You can change the size of dx to make an even better fit. But yes, numerical integrations can be fairly easy—and useful.</p>

			<a class="visually-hidden skip-to-text-link focusable bg-white" href="#start-of-content">Go Back to Top. Skip To: Start of Article.</a>

			
</div>
<br>[ad_2]
<br><a href="http://feeds.wired.com/c/35185/f/661370/s/4db0c8f3/sc/27/l/0L0Swired0N0C20A160C0A20Cdominate0Ecalculus0Ewith0Ea0Efew0Eeasy0Etricks0C/story01.htm">Source </a>