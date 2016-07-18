---
ID: 1716
post_title: >
  The Physics of Buster’s Epic End in
  the MythBusters Finale
author: Staff Writer
post_date: 2016-03-10 15:22:12
post_excerpt: ""
layout: post
permalink: >
  https://www.whenitson.com/the-physics-of-busters-epic-end-in-the-mythbusters-finale/
published: true
original_cats:
  - >
    Science Blogs,mythbusters,g-forces,Dot
    Physics,Acceleration,video
    analysis,Science
original_title:
  - >
    The Physics of Buster’s Epic End in
    the MythBusters Finale
original_link:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4e2b94c5/sc/27/l/0L0Swired0N0C20A160C0A30Cphysics0Ebusters0Eepic0Eend0Emythbusters0Efinale0C/story01.htm
canonical_url:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4e2b94c5/sc/27/l/0L0Swired0N0C20A160C0A30Cphysics0Ebusters0Eepic0Eend0Emythbusters0Efinale0C/story01.htm
---
 [ad_1]
<br><div id=""><p>After 14 epic years, the MythBusters have aired their final episode. But just because the show has ended doesn’t mean the analysis has to stop. Actually, you could probably go back through all the <em>MythBusters</em> episodes and find quite a few examples that pose some interesting physics questions.</p>
<p>We won’t go back that far for this analysis. In the <em>MythBusters</em> finale, everyone figured they should send Buster (the crash test dummy) out with style. They mounted him to a rocket sled and crashed him into a wall with a speed of approximately 800 mph. There was pretty much nothing left of Buster after the impact.</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/03/The-Physics-of-Busters-Epic-End-in-the-MythBusters-Finale.gif" alt="Busterrocket 1" width="558" height="307"/></p>
<p>Instead of looking at the impact, let’s focus on the rocket-based acceleration part. For my first approximation of the acceleration, I will use just two things—the length of the track and the time of the acceleration. Other than that, I can make the following assumptions:</p>
<ul><li>The rocket sled starts from rest—this seems to be obviously true.</li>
<li>The acceleration of the rocket sled is constant. This is most likely not exactly true, but it should be close enough to constant for this estimation.</li>
</ul><p>Now I need two pieces of information. For the length of the track, I am going to use 300 meters—since that’s what’s listed on <a href="http://www.emrtc.nmt.edu/facilities/sledtrack.php">New Mexico Tech’s Energetic Materials and Research Testing Center</a>. But what about the time? If I assume a couple of the shots of the sled are in “real time,” then I can just count video frames to get an acceleration time of 1.16 seconds.</p>
<p>To find the acceleration, I could just use the kinematic equations—but that’s boring. Instead, let’s start with the definition of acceleration and average velocity in 1-dimension:</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/03/The-Physics-of-Busters-Epic-End-in-the-MythBusters-Finale.jpg" alt="La te xi t 1" width="189" height="117"/></p>
<p>Notice that there are actually two definitions for the average velocity. It is equal to the change in position divided by the change in time—but it is also the average of the starting and ending velocity. If the rocket starts from rest, I can set v<sub>1</sub> = 0 m/s. Now using the definitions of average velocity, I can get an expression for the final velocity.</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/03/1457623332_790_The-Physics-of-Busters-Epic-End-in-the-MythBusters-Finale.jpg" alt="La te xi t 1" width="176" height="121"/></p>
<p>Using this expression for the final velocity, I get the following for the acceleration:</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/03/1457623332_859_The-Physics-of-Busters-Epic-End-in-the-MythBusters-Finale.jpg" alt="La te xi t 1" width="188" height="86"/></p>
<p>Using my values for Δx and Δt, I get an acceleration of 446 m/s<sup>2</sup> or 45.5 g’s. That’s a pretty large acceleration. In fact, if Buster was a normal human he wouldn’t have to worry about crashing into a wall—he would probably be dead just due to the rockets.</p>
<p>What about the final speed on impact? If use the same definition of average acceleration, the final velocity would be:</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/03/1457623332_838_The-Physics-of-Busters-Epic-End-in-the-MythBusters-Finale.jpg" alt="La te xi t 1" width="131" height="49"/></p>
<p>With the same value for the time interval and the above value for acceleration, this puts the final speed at 517 m/s (1156 mph). That’s not fast—that’s damn fast.</p>
<p>Later in the clip, there is an aerial view of the rocket sled.</p>
<p><img class="aligncenter" src="http://www.whenitson.com/wp-content/uploads/2016/03/1457623332_480_The-Physics-of-Busters-Epic-End-in-the-MythBusters-Finale.gif" alt="Rocket 2" width="558" height="307"/></p>
<p>I can use this to get both position and time data from the video. Normally, I would like the motion of the object perpendicular to the camera’s view—but in this case the camera is far enough away that I can ignore effects due to perspective distortion.</p>
<p>Here is the plot of the position of the sled along the track.</p>
<p><a href="http://www.wired.com/wp-content/uploads/2016/03/data_tool21.jpg"><img class="aligncenter wp-image-1985117 size-text-column-width" src="http://www.whenitson.com/wp-content/uploads/2016/03/1457623332_74_The-Physics-of-Busters-Epic-End-in-the-MythBusters-Finale.jpg" alt="data_tool21.jpg" width="482" height="392"/></a></p>
<p>It seems like the data fits a parabolic equation quite nicely. This is what you would expect for an object with a constant acceleration (like I assumed earlier). Also, looking at the coefficient in front of the t<sup>2</sup> term, I can find the acceleration with a value of 389.2 m/s<sup>2</sup>. Yes, this is a little bit different than my acceleration value from my previous attempt. However, they are close enough to make me happy.</p>

			<a class="visually-hidden skip-to-text-link focusable bg-white" href="#start-of-content">Go Back to Top. Skip To: Start of Article.</a>

			
</div>
<br>[ad_2]
<br><a href="http://feeds.wired.com/c/35185/f/661370/s/4e2b94c5/sc/27/l/0L0Swired0N0C20A160C0A30Cphysics0Ebusters0Eepic0Eend0Emythbusters0Efinale0C/story01.htm">Source </a>