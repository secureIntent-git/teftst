---
ID: 2712
post_title: >
  The Physics of That Crazy Ricochet Hole
  in One at the Masters
author: Staff Writer
post_date: 2016-04-12 22:02:07
post_excerpt: ""
layout: post
permalink: >
  https://www.whenitson.com/the-physics-of-that-crazy-ricochet-hole-in-one-at-the-masters/
published: true
original_cats:
  - >
    numerical
    calculation,Python,Momentum,Science
    Blogs,Dot
    Physics,golf,collisions,estimation,Science
original_title:
  - >
    The Physics of That Crazy Ricochet Hole
    in One at the Masters
original_link:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4ee54323/sc/13/l/0L0Swired0N0C20A160C0A40Cphysics0Ecrazy0Ericochet0Ehole0Eone0Emasters0C/story01.htm
canonical_url:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4ee54323/sc/13/l/0L0Swired0N0C20A160C0A40Cphysics0Ecrazy0Ericochet0Ehole0Eone0Emasters0C/story01.htm
---
 [ad_1]
<br><div id=""><blockquote class="twitter-tweet" data-width="500" readability="5.7169811320755"><p lang="en" dir="ltr">Watch <a href="https://twitter.com/Louis57TM">@Louis57TM</a> make a hole-in-one off J.B. Holmes golf ball on No. 16 <a href="https://twitter.com/hashtag/themasters?src=hash">#themasters</a> <a href="https://t.co/gQUlT7t62K">https://t.co/gQUlT7t62K</a></p>
<p>— Masters Tournament (@TheMasters) <a href="https://twitter.com/TheMasters/status/719270992401412096">April 10, 2016</a></p></blockquote>

<p>It’s not so easy to get a hole in one—you can’t control every part of a ball’s motion towards the hole. So, let’s say this shot is part skill and part luck. In case you missed it, Louis Oosthuizen took a shot on a par 3 hole at the US Masters in Augusta this weekend. It was a nice shot, but it most likely would not have gone in the hole without first colliding with a ball from the previous shot.</p>
<p>Is there some cool physics here? Yes. Let’s get to some questions.</p>
<h3>Is momentum conserved in a ball collision?</h3>
<p>What is momentum? It’s simply the product of an object’s mass and velocity. This is very important in the momentum principle. It states that a force changes an object’s momentum. In one dimension, this can be written as:</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/04/The-Physics-of-That-Crazy-Ricochet-Hole-in-One-at-the-Masters.jpg" alt="La te xi t 1" width="126" height="69"/></p>
<p>Now for the cool part. When one ball collides with another ball, it pushes on it. However, forces always come in pairs so that the stationary ball pushes back on the moving ball with the exact same force (but in the opposite direction). Since the two balls are in contact for the same time with the same (but opposite) force, they have opposite changes in momentum. Or, we can say that the total momentum before is equal to the total momentum after the collision. This is called conservation of momentum.</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/04/1460498527_927_The-Physics-of-That-Crazy-Ricochet-Hole-in-One-at-the-Masters.jpg" alt="Spring 2016 Sketches key" width="399" height="197"/></p>
<p>Of course these golf balls are moving in two dimensions. So, momentum is conserved in both the x and y-directions. But what about the frictional force from the grass? What about the gravitational force pulling the ball down the incline? Yes, both of these matter. However, the collision is during such a short time interval that these other forces don’t matter much if you look at RIGHT before the collision and RIGHT after the collision.</p>
<h3>How did a deflection put the ball in the hole?</h3>
<p>Now for the important question. What happened here? Let me call the moving ball, ball A and initially stationary ball, ball B. It might look like the collision made ball A increase in speed, but I don’t think so. Here’s what happened. Ball A was moving sort of towards the hole and then collided with ball B. After the collision, ball A deflected to the right and went uphill a bit. Since it was going slower after the collision, it had more time after the hit for the slight downward slope to curve its trajectory back to the hole. Hole in one.</p>
<p>OK, my description might not make too much sense. Let me model it instead. As I like to say—you don’t really understand something unless you can model it. This is a numerical calculation with two important interactions.</p>
<ul><li>First, there is a slight downward gravitational force. In this model, I have the slope of the grass at some constant value. The direction downhill is same as the vector &lt;-1, 1, 0&gt; (in the python program, positive y is towards the top of your screen).</li>
<li>Second, what about the collision between the two balls? Here I used a simple spring-based collision model. If the two balls are closer than twice their radius, there is a force pushing them away that is proportional to the overlap distance. I have <a href="http://www.wired.com/2013/11/modeling-a-one-dimensional-collision/">an older post describing this</a>, but maybe I should make a new one with better code.</li>
</ul><p>That’s pretty much it. I guessed at some of the initial parameters (like position of ball B and initial speed of ball A). Other than that, I did have to determine the best angle to launch ball A so that it would hit ball B <em>just</em> right. To find this optimal angle, I just reran my numerical calculation many times and changed the starting angle until I found the value that resulted in a hole in one.</p>
<p>OK, here is the code. You probably just want to push the play button to run it. In case you can’t tell, I am letting the green circle represent the hole.</p>

<p>Pretty cool, right?</p>
<h3>What are the chances of something like this happening?</h3>
<p>OK, that’s not the best question. Really the only way to estimate the probability of something like this is to run a bunch of numerical calculations and count how many of them result in the same outcome. The problem is that we don’t really know the input paramenters. If one golf hit a ball 1,000 times, what kind of variation in outcomes would you get? I guess you could do this experimentally, but it would be tough. On top of that, you would have to take into account external factors like wind and the exact shape of the grass around the hole.</p>
<p>Instead, let me calculate something else. Suppose a golf ball starts 2 meters away from another stationary ball. What range of starting velocity angles will result in a collision between these two balls? I’m just looking for a collision, not a collision that results in a hole in one.</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/04/1460498527_951_The-Physics-of-That-Crazy-Ricochet-Hole-in-One-at-the-Masters.jpg" alt="Spring 2016 Sketches key" width="619" height="198"/></p>
<p>In this diagram (which is not to scale), you can see that the range of possible trajectories that lead to a collision create a triangle. If the size of the ball is much smaller than the starting distance, then this is just like a typical angular size problem that we see in astronomy. If the starting distance is <em>L</em> and the diameter of the ball is <em>d</em> then:</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/04/1460498527_511_The-Physics-of-That-Crazy-Ricochet-Hole-in-One-at-the-Masters.jpg" alt="La te xi t 1" width="111" height="72"/></p>
<p>Now I can put in my values. I already said that the starting distance was 2 meters. We also know the diameter of a golf ball is about 43 mm (0.043 meters). Using both of these values I get an angular width of 0.043 radians (2.5 degrees). That’s not too difficult to hit, but it’s only 2 meters away. If you increase the starting distance to something larger, like 4 meters the angle drops to half that value at 0.0215 radians (1.2 degrees). What if you want to hit that ball from the start of the par 3 hole? Let’s use a distance of 200 yards (183 m). This would give an angular target size of just 0.027 degrees. That’s a pretty small target. And remember, that’s to just hit the stationary ball, not get a hole in one.</p>
<p>If you want a homework assignment, you can run the numerical calculation above and find the range of starting ball velocity angles that will result in a hole in one. I bet the range is pretty small.</p>

			<a class="visually-hidden skip-to-text-link focusable bg-white" href="#start-of-content">Go Back to Top. Skip To: Start of Article.</a>

			
</div>
<br>[ad_2]
<br><a href="http://feeds.wired.com/c/35185/f/661370/s/4ee54323/sc/13/l/0L0Swired0N0C20A160C0A40Cphysics0Ecrazy0Ericochet0Ehole0Eone0Emasters0C/story01.htm">Source </a>