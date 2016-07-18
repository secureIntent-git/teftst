---
ID: 748
post_title: >
  Tackle a Runner Like a Super Bowl
  Player—With Physics!
author: Staff Writer
post_date: 2016-02-06 07:51:24
post_excerpt: ""
layout: post
permalink: >
  https://www.whenitson.com/tackle-a-runner-like-a-super-bowl-player-with-physics/
published: true
original_cats:
  - >
    numerical model,Python,Science
    Blogs,physics,Velocity,Superbowl,Dot
    Physics,nfl,Science
original_title:
  - >
    Tackle a Runner Like a Super Bowl
    Player—With Physics!
original_link:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4d65b445/sc/35/l/0L0Swired0N0C20A160C0A20Ctackle0Ea0Erunner0Elike0Ea0Esuper0Ebowl0Eplayer0Ewith0Ephysics0C/story01.htm
canonical_url:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4d65b445/sc/35/l/0L0Swired0N0C20A160C0A20Ctackle0Ea0Erunner0Elike0Ea0Esuper0Ebowl0Eplayer0Ewith0Ephysics0C/story01.htm
---
 [ad_1]
<br><div id=""><p>You are a football player on defense. Some guy on offense just caught the ball and you are the only person that can catch him. You can run a little bit faster than him and both of you are on the 50 yard line. So, how do you catch him? What path should you run? Here are three approaches.</p>
<h3>The Math Method</h3>
<p>Ok, a couple of assumptions. The wide receiver has the ball and he can run 6.5 m/s. He is completely obsessed with scoring a touchdown. He’s so focused that he runs in a straight line without turning. You can run at a speed of 7.0 m/s but you are 5 meters to the right of him. Both of you accelerate up to maximum speed right away.</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/02/Tackle-a-Runner-Like-a-Super-Bowl-PlayerWith-Physics.jpg" alt="Spring 2016 Sketches key" width="510" height="245"/></p>
<p>Since you have plenty of time to plan your attack, you quickly estimate your opponent’s speed and distance. With that you calculate your optimal angle to intercept him in the shortest distance. So, what angle should you aim for?</p>
<p>Let’s think of both players as having motion in both the x and y direction (with the y-direction towards the end zone). Player one has the ball. He has no motion in the x-direction so that we can express his position as a function of time as:</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/02/1454745084_119_Tackle-a-Runner-Like-a-Super-Bowl-PlayerWith-Physics.jpg" alt="La te xi t 1" width="109" height="49"/></p>
<p>This assumes that he starts at the origin at time <em>t</em> = 0 seconds and his speed is <em>v</em><sub>2</sub>. For player two (I guess that would be you), there is a motion in both the x- and y-directions. I can use the angle θ to find the components of velocity and the equations of motion. Let me say that you start at a position of <em>x</em><sub>0</sub> (which I said would be 5 m).</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/02/1454745084_173_Tackle-a-Runner-Like-a-Super-Bowl-PlayerWith-Physics.jpg" alt="La te xi t 1" width="191" height="79"/></p>
<p>If you solve these three equations for the point where both have the same <em>x</em> and <em>y</em> at the same time, you get a solution of:</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/02/1454745084_538_Tackle-a-Runner-Like-a-Super-Bowl-PlayerWith-Physics.jpg" alt="La te xi t 1" width="181" height="117"/></p>
<p>Does this answer make sense? First, what would happen if the offensive guy was faster? There would be no angle you could use to catch him, right? Can you take the inverse sine of a value greater than one? Nope. That’s good. But what’s weird? The solution does not depend on the horizontal separation. Does that mean it doesn’t matter? No—it will take longer to catch him the farther you start—but the angle is the same.</p>
<p>Here is a numerical model of this situation (just click the play button to start it).</p>

<p>It’s on <a href="http://trinket.io">trinket.io</a> so feel free to look at the code and change it to see what happens. Try different starting positions and velocities. Note that this gives an optimal angle of 68.2 degrees and it takes a distance of 12 meters to catch him.</p>
<p>I should point out that this solution does indeed work—but it’s not realistic. You can’t calculate inverse sine functions in your head. You might be pretty good at estimating the angle to run to meet the other guy at the right spot, but you don’t actually calculate anything.</p>
<h3>The Aiming Method</h3>
<p>Here is another way to catch the receiver—run as fast as you can and always run towards the other player. This means that you would start off with a velocity in the negative x-direction but then as the player moved up you would start aiming up. How far would you need to go to catch him? That’s not such an easy calculation. However, it’s not too difficult to make a numerical model. Before showing you the code, let me include one diagram.</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/02/1454745084_934_Tackle-a-Runner-Like-a-Super-Bowl-PlayerWith-Physics.jpg" alt="Spring 2016 Sketches key" width="307" height="250"/></p>
<p>Here is the plan. In each step of my program I am going to calculate the vector from player two to player one (I call this vector <em>r</em>). I will then set the velocity of player one to be equal to a vector in the same direction as <em>r</em> (r-hat is the unit vector) with a magnitude of <em>v</em><sub>2</sub>. It’s not too difficult. Here is the code for this run (again, just press the play thingy).</p>

<p>You can see that for the same starting conditions, this one lets the player run much farther before being tackled (31.3 meters vs. 12 meters). It’s an easy way to run since you just aim at the target, but it’s not quite as effective. If a football player runs this way, he shouldn’t be in the NFL.</p>
<h3>The Thinking Ahead Method</h3>
<p>What if you aim a little bit ahead of the player instead of right at him? We need a plan. Let’s start with a diagram again.</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/02/1454745084_994_Tackle-a-Runner-Like-a-Super-Bowl-PlayerWith-Physics.jpg" alt="Spring 2016 Sketches key" width="459" height="281"/></p>
<p>This looks crazy, but let me explain. Here’s how we will do it.</p>
<ul><li>Calculate the vector distance between the two players.</li>
<li>Use this distance along with the speed of player 2 to calculate the time it would take for this player to get there (call this time Δt).</li>
<li>Using the time interval (Δt) find out how far ahead player 1 would move during this time. I am representing this new position with a small dot.</li>
<li>Now use the same dumb aiming method from before but aim at the small dot instead of the player.</li>
<li>Recalculate every time you move.</li>
</ul><p>The awesome thing is that as the two players get closer, the “aim ahead point” gets closer to the actual player. With this, you shouldn’t miss. Here is the code for this motion.</p>

<p>He caught the runner is just 17.5 meters. That’s not as good as the mathematical method, but much better than the running-like-a-dog-at-a-rabbit method. Feel free to and change the code and make your own model.</p>
<h3>Homework</h3>
<p>So many unanswered questions. Here are a few.</p>
<ul><li>What if the offensive player decides to turn? Which method would work the best in this case?</li>
<li>Suppose you are now the guy with the ball running for a touchdown. What should you do? Clearly if a defensive player uses the first math method any little change will make him miss. But what about the other methods? Can you create some running algorithm that will maximize the distance before he catches you? Remember you have to stay in bounds.</li>
<li>What would change if the two players don’t start at the same yard line? What if the runner starts 5 meters ahead? What if the defensive guy starts ahead?</li>
<li>What about two defensive players? This is getting pretty close to the <a href="http://www.wired.com/2015/10/heres-solve-xkcd-velociraptor-problem-code/">velociraptor problem that I never finished</a> (but I will).</li>
</ul><a class="visually-hidden skip-to-text-link focusable bg-white" href="#start-of-content">Go Back to Top. Skip To: Start of Article.</a>

			
</div>
<br>[ad_2]
<br><a href="http://feeds.wired.com/c/35185/f/661370/s/4d65b445/sc/35/l/0L0Swired0N0C20A160C0A20Ctackle0Ea0Erunner0Elike0Ea0Esuper0Ebowl0Eplayer0Ewith0Ephysics0C/story01.htm">Source </a>