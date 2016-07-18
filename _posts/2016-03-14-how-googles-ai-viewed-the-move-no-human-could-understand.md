---
ID: 1823
post_title: >
  How Google’s AI Viewed the Move No
  Human Could Understand
author: Staff Writer
post_date: 2016-03-14 07:09:09
post_excerpt: ""
layout: post
permalink: >
  https://www.whenitson.com/how-googles-ai-viewed-the-move-no-human-could-understand/
published: true
original_cats:
  - >
    Enterprise,Artificial
    Intelligence,AlphaGo,David
    Silver,reinforcement learning,Korea,Fan
    Hui,Lee Sedol,google,Seoul,deep
    learning,Demis
    Hassabis,DeepMind,Business
original_title:
  - >
    How Google’s AI Viewed the Move No
    Human Could Understand
original_link:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4e3dbbad/sc/13/l/0L0Swired0N0C20A160C0A30Cgoogles0Eai0Eviewed0Emove0Eno0Ehuman0Eunderstand0C/story01.htm
canonical_url:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4e3dbbad/sc/13/l/0L0Swired0N0C20A160C0A30Cgoogles0Eai0Eviewed0Emove0Eno0Ehuman0Eunderstand0C/story01.htm
---
 [ad_1]
<br><div id=""><p>SEOUL, SOUTH KOREA — The move didn’t make sense to all the humans packed into the sixth floor of Seoul’s Four Seasons hotel. But the Google machine saw it quite differently. The machine knew the move wouldn’t make sense to all those humans. Yes, it knew. And yet it played the move anyway, because this machine has seen so many moves that no human ever has.  </p>
<p>In the <a href="http://www.wired.com/2016/03/googles-ai-wins-pivotal-game-two-match-go-grandmaster/" target="_blank">second game</a> of <a href="http://www.wired.com/2016/03/googles-ai-taking-one-worlds-top-go-players/" target="_blank">this week’s historic Go match</a> between Lee Sedol, one of the world’s top players, and AlphaGo, an artificially intelligent computing system built by a small team of Google researchers, this surprisingly skillful machine made a move that flummoxed everyone from the throngs of reporters and photographers to the match commentators to, yes, Lee Sedol himself. “That’s a very strange move,” said one commentator, an enormously talented Go player in his own right. “I thought it was a mistake,” said the other. And Lee Sedol, after leaving the match room for a spell, needed nearly fifteen minutes to settle on a response.</p>
<p>Fan Hui, the three-time European Go champion <a href="http://www.wired.com/2016/01/in-a-huge-breakthrough-googles-ai-beats-a-top-player-at-the-game-of-go/" target="_blank">who lost five straight games to AlphaGo this past October</a>, was also <a href="http://www.wired.com/2016/03/sadness-beauty-watching-googles-ai-play-go/" target="_blank">completely gobsmacked</a>. “It’s not a human move. I’ve never seen a human play this move,” he said. But he also called the move “So beautiful. So beautiful.” Indeed, it changed the path of play, and AlphaGo went on to win the second game. Then it won the third, <a href="http://www.wired.com/2016/03/third-straight-win-googles-ai-claims-victory-historic-match-go-champ/" target="_blank">claiming victory in the best-of-five match after a three-game sweep</a>, before Lee Sedol <a href="http://www.wired.com/2016/03/go-grandmaster-lee-sedol-grabs-consolation-win-googles-ai/" target="_blank">clawed back a dramatic win in Game Four</a> to save a rather large measure of human pride.</p>
<p>It was a move that demonstrated the mysterious power of modern artificial intelligence, which is not only driving one machine’s ability to play this ancient game at an unprecedented level, but simultaneously reinventing <a href="http://www.wired.com/2016/03/googles-ai-taking-one-worlds-top-go-players/" target="_blank">all of Google</a>—<a href="http://www.wired.com/2015/12/elon-musks-billion-dollar-ai-plan-is-about-far-more-than-saving-the-world/" target="_blank">not to mention Facebook and Microsoft and Twitter and Tesla and SpaceX</a>. In the wake of Game Two, Fan Hui so eloquently described the importance and the beauty of this move. Now an advisor to the team that built AlphaGo, he spent the last five months playing game after game against the machine, and he has come to recognize its power. But there’s another player who has an even greater understanding of this move: AlphaGo. </p>
<p>I was unable to ask AlphaGo about the move. But I did the next best thing: I asked David Silver, the guy who led the creation of AlphaGo.</p>
<figure attachment_1987742="" class="wp-caption landscape alignnone  relative" data-js="fader"><a href="http://www.wired.com/wp-content/uploads/2016/03/GW20160133481.jpg"><img src="http://www.whenitson.com/wp-content/uploads/2016/03/How-Googles-AI-Viewed-the-Move-No-Human-Could-Understand.jpg" alt="David Silver. " width="1024" height="768" class="size-large wp-image-1987742"/></a><figcaption class="wp-caption-text link-underline">David Silver.  <span class="credit link-underline-sm"><span aria-hidden="true" class="ui ui ui-photo inline-block ui-credit relative opacity-5 marg-r-micro"/> Geordie Wood for WIRED</span></figcaption></figure><h3>‘It’s Hard to Know Who To Believe’</h3>
<p>Silver is a researcher at a London AI lab called DeepMind, which Google acquired in early 2014. He and the rest of the team that built AlphaGo arrived in Korea well before the match, setting up the machine—and its all important Internet connection—inside the Four Seasons, and in the days since, they’ve worked to ensure the system is in good working order before each game, while juggling interviews and photo ops with the throng of international media types.</p>
<p>But they’re mostly here to <em>watch the match</em>—much like everyone else. One DeepMind researcher, Aja Huang, is actually in the match room during games, physically playing the moves that AlphaGo decrees. But the other researchers, including Silver, are little more than spectators. During a game, AlphaGo runs on its own.   </p>
<p>That’s not to say that Silver can relax during the games. “I can’t tell you how tense it is,” Silver tells me just before Game Three. During games, he sits inside the AlphaGo “control room,” watching various computer screens that monitor the health of the machine’s underlying infrastructure, display its running prediction of the game’s outcome, and provide live feeds from various match commentaries playing out in rooms down the hall. “It’s hard to know what to believe,” he says. “You’re listening to the commentators on the one hand. And you’re looking at AlphaGo’s evaluation on the other hand. And all the commentators are disagreeing.” </p>
<p>During Game Two, when Move 37 arrived, Silver had no more insight into this moment than anyone else at the Four Seasons—or any of the millions watching the match from across the Internet. But after the game and all the effusive praise for the move, he returned to the control room and did a little digging.</p>
<h3>Playing Against Itself</h3>
<p>To understand what he found, you must first understand how AlphaGo works. Initially, Silver and team taught the system to play the game using what’s called a deep neural network—a network of hardware and software that mimics the web of neurons in the human brain. This is the same basic technology that identifies faces in photos uploaded to Facebook or recognizes commands spoken into Android phones. If you feed enough photos of a lion into a neural network, it can learn to recognize a lion. And if you feed it millions of Go moves from expert players, it can learn to play Go—a game that’s exponentially more complex than chess. But then Silver and team went a step further.</p>
<p>Using a second technology called reinforcement learning, they set up matches in which slightly different versions of AlphaGo <em>played each other</em>. As they played, the system would track which moves brought the most reward—the most territory on the board. “AlphaGo learned to discover new strategies for itself, by playing millions of games between its neural networks, against themselves, and gradually improving,” Silver said <a href="http://www.wired.com/2016/01/in-a-huge-breakthrough-googles-ai-beats-a-top-player-at-the-game-of-go/" target="_blank">when DeepMind first revealed the approach earlier this year</a>. </p>
<p>And then the team went a step further than that. They fed moves from these AlphaGo-versus-AlphaGo matches into <em>another neural network</em>, refining its play still more. Basically, this neural network trained the system to look ahead to the potential results of each move. With this training, combined with a “tree search” examines the potential outcomes in a more traditional and systematic, it estimates the probability that a given move will result in a win.</p>
<p>So, in the end, the system learned not just from human moves but from moves generated by multiple versions of itself. The result is that the machine is capable of something like Move 37. </p>
<h3>A One in Ten Thousand Probability</h3>
<p>Following the game, in the control room, Silver could revisit the precise calculations AlphaGo made in choosing Move 37. Drawing on its extensive training with millions upon millions of human moves, the machine actually calculates the probability that a human will make a particular play in the midst of a game. “That’s how it guides the moves it considers,” Silver says. For Move 37, the probability was <em>one in ten thousand</em>. In other words, AlphaGo knew this was not a move that a professional Go player would make. </p>
<p>But, drawing on all its other training with millions of moves generated by games with itself, it came to view Move 37 in a different way. It came to realize that, although no professional would play it, the move would likely prove quite successful. “It discovered this for itself,” Silver says, “through its own process of introspection and analysis.”</p>
<p>Is introspection the right word? You can be the judge. But Fan Hui was right. The move was inhuman. But it was also beautiful.</p>

			<a class="visually-hidden skip-to-text-link focusable bg-white" href="#start-of-content">Go Back to Top. Skip To: Start of Article.</a>

			
</div>
<br>[ad_2]
<br><a href="http://feeds.wired.com/c/35185/f/661370/s/4e3dbbad/sc/13/l/0L0Swired0N0C20A160C0A30Cgoogles0Eai0Eviewed0Emove0Eno0Ehuman0Eunderstand0C/story01.htm">Source </a>