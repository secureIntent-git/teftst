---
ID: 2525
post_title: >
  Here’s How Google Makes Sure It
  (Almost) Never Goes Down
author: Staff Writer
post_date: 2016-04-06 17:39:07
post_excerpt: ""
layout: post
permalink: >
  https://www.whenitson.com/heres-how-google-makes-sure-it-almost-never-goes-down/
published: true
original_cats:
  - >
    Enterprise,DevOps,code,google,Business,software
original_title:
  - >
    Here’s How Google Makes Sure It
    (Almost) Never Goes Down
original_link:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4ec3ad08/sc/15/l/0L0Swired0N0C20A160C0A40Cgoogle0Eensures0Eservices0Ealmost0Enever0Ego0C/story01.htm
canonical_url:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4ec3ad08/sc/15/l/0L0Swired0N0C20A160C0A40Cgoogle0Eensures0Eservices0Ealmost0Enever0Ego0C/story01.htm
---
 [ad_1]
<br><div id=""><p>When was the last time you needed to Google something and Google wasn’t there?</p>
<p>Odds are, you don’t remember that ever happening. Sure, there are times when you can’t reach Google because your internet connection is down. But Google’s primary online services, from its search engine to Gmail to Google Docs and more, are nearly always accessible. The company’s Google Apps suite, including Gmail and Docs, was available about 99.97 percent of the time in 2015, according to the company’s own numbers. The world pretty much takes this for granted, but it’s a remarkable reality. The billions who use Google hardly stop to consider how Google made something so impressive seem so mundane.</p>
<p>Google explains the feat in three words: Site Reliability Engineering. OK, they aren’t the best three words. But that’s the rather unsexy name Google gave to this seminal philosophy more than a decade ago. It’s a rather nuanced and expansive philosophy, but it really boils down to one central idea: <em>Don’t get IT people who specialize in running Internet services to run your Internet services. Have software coders run them instead</em>. If you do this, the thinking goes, the software coders will build tools that can help run the operation <em>without the active involvement of real live people</em>.</p>
<p data-js="fader" class="pullquote carve fader">
	'We long for the day when nobody runs anything.'	<span class="attribution">Todd Underwood, Google</span>
</p>

<p>“The result of our approach,” writes Googler Ben Treynor Sloss in a new essay, “is that we end up with a team of people who will quickly become bored by performing tasks by hand and have the skill set necessary to write software to replace their previously manual work.”</p>
<p>For many in Silicon Valley, that may seem like a common idea. This kind of thing is now practiced across the tech world, from Amazon to Box.com. People call it DevOps—“development” plus “operations”—an effort to combine the ways of the software coder with the aims of the systems administrator. But the DevOps movement, embodied by tools like Chef and Puppet, <a href="http://www.wired.com/2011/10/chef_and_puppet/" target="_blank">evolved separately from and largely after</a> the SRE philosophies that arose inside Google (and similar ideas that took hold at Amazon). It’s just that Google has kept largely quiet about this over the last decade, as it <a href="http://www.wired.com/2012/08/google-as-xerox-parc/" target="_blank">often did when the topic was the inner workings of its enormously efficient online operation</a>. </p>
<p>But the company has entered a new period, one in which it’s more willing to discuss such things (<a href="http://www.wired.com/2014/03/urs-google-story/" target="_blank">mainly because it wants to promote the cloud services that allow outside business to run their own software atop its vast network of data centers and machines</a>). Google has even gone so far as to write a book about Site Reliability Engineering.</p>
<p>The book is called, well, <em>Site Reliability Engineering</em>. It was just <a href="http://shop.oreilly.com/product/0636920041528.do" target="_blank">published by O’Reilly</a>, and the essay from Sloss serves as the first chapter. If you’re into DevOps, it’s a must-read. And even if you’re not, the opening of the book—the preface, the introduction, and the first chapter–is a fascinating look at the attitudes that drive the world’s largest online empire.</p>
<p>For many in tech—and almost everyone outside of tech—system administration (or operations or whatever you want to call it) is an afterthought, one of the more boring aspects of computer technology. But Sloss, officially known as Google’s Vice President for 24/7 Operations, turns this notion upside down, arguing that site reliability is “the most fundamental feature of any product.” After all: “A system isn’t very useful if nobody can use it.”</p>
<h3>Ground Zero</h3>
<p>Sloss is ground zero for the SRE movement. It began when Google hired him to run its operations, and it was he who coined the term. “SRE is what happens when you ask a software engineer to design an operations team,” he says. “I designed and managed the group the way I would want it to work if I worked as an SRE myself.”</p>
<p>For Todd Underwood, now an SRE director at Google, it’s only natural that the company would hire a coder like Sloss for the job. “When Google was in its infancy, there were so many software engineers who had a better sense of how things broke and a better sense of how engineering could be done well,” he tells WIRED. “But not one them wanted to do any of that by hand.”</p>
<p>That’s a very Googly thing to say. But Adam Jacob, chief technology officer at Chef, pretty much agrees, explaining that this is the expected transition for an online operation that’s growing to such a large size. “It’s natural to have a conversation to combine software development and the practical pieces of operation—and to have no real divide between the two,” he says. “When you look at the problem holistically, you get better results.”</p>



<p>The shift is particularly interesting when you consider that dev and ops were traditionally opposing forces. The devs wanted to build new software and change it and get the changes out to the public as a fast as possible. But the ops folks wanted to ensure that nothing went wrong, and the best way to do that was to keep changes to a minimum. “These are incommensurate goals,” Underwood says. The trick is that, if you combine dev and ops, you can start to eliminate their competing aims.</p>
<p>Underwood calls it a “Hegelian thesis-antithesis synthesis.” He then acknowledges that when he says this, no one really buys it. “People just don’t read Hegel anymore,” he quips. But the description is spot on. And once this synthesis was in place, Google accelerated the process by adding all sorts of other Googly ideas to the mix.</p>
<h3>The Error Budget</h3>
<p>One big idea is that, in an effort to reduce the conflict between dev and ops, the company doesn’t strive for 100 percent uptime. The reality, Sloss writes, is that you don’t need an internet service to be 100 percent available. Users can’t really tell the difference between 100 percent and, say, 99.999 percent (their laptop or WiFi or electricity or ISP are down far more than 0.001 percent of the time). If you set a reasonable uptime goal below 100 percent—an “error budget”—you have more room to make changes and role out experiments.</p>
<p>“The use of an error budget resolves the structural conflict of incentives between development and SRE,” Slosser says. “An outage is no longer a ‘bad’ thing. It is an expected part of the process of innovation, and an occurrence that both development and SRE teams manage rather than fear.”</p>
<p>At the same time, the company put rules in place to ensure that SREs didn’t end up morphing into good old fashioned sysadmins. Basically, it decreed that no SRE could spent more than 50 percent of his or her time on traditional operations as opposed to coding. If ops starts to take precedence over dev on a particular SRE team, Google shifts some of the ops load onto the team that is typically just build the software—the regular Google software engineers. “Consciously maintaining this balance between ops and development work allows us to ensure that SREs have the bandwidth to engage in creative, autonomous engineering,” Sloss writes, “while still retaining the wisdom gleaned from the operations side of running a service.”</p>
<p>Chef’s Jacob says that the ratio here—50 percent—isn’t that important. But he likes the attitude. “This is just economics,” he says. “There’s always demand for people to do operational bullshit. There is an almost infinite amount of bullshit that people will ask an operational person to do. So the idea that you would put a cap on that it legit.”</p>
<p>Google even created strict guidelines for hiring its SREs. It hires about 50 to 60 percect through exactly the same process that applies to all other Google engineers, and the rest have about “85 to 99 percent” of the same skills—plus a “set of technical skills that is useful to SRE but is rare for most software engineers,” such as an intimate knowledge of the inside of the UNIX operating system or hardware networking protocols. This too aims to ensure that dev and ops maintain the proper balance. </p>
<h3>The Moonshot That Keeps Google Online</h3>
<p>In many ways, this was a new philosophy. But in their book, as they seek to describe the philosophy, the Google team uses a much older example. The spiritual forebear of the Google SREs is Margaret Hamilton, <a href="http://www.wired.com/2015/10/margaret-hamilton-nasa-apollo/" target="_blank">the MIT programmer who spent the ’60s building software for Apollo spacecraft that would one day land on the moon</a>. As explained by Hamilton herself—who was interviewed for the book—part of the culture on the Apollo program “was to learn from everyone and everything, including from that which one would least expect.”</p>
<p>Hamilton was a coder. But she played an important role in operations. To show this, the book recounts the day Hamilton’s young daughter, Lauren, who she often brought to the computer lab, happened to hit a button and feed an Apollo pre-launch program into a computer that was running a post-launch scenario.</p>
<p>This crashed the scenario, and Hamilton tried to add a new error checking code to the system that automatically would prevent this during a real flight. Her superiors rejected the idea, arguing that astronauts would never do such a thing, but on Apollo 8, the astronauts did such a thing. Luckily, Hamilton had added a workaround to the system documentation. And for subsequent missions, she added the error checking code.</p>
<p>“If you come along and say ‘That’s going to break,’ it’s really not that useful. But if say: ‘That’s going to break, and let me tell you how,’ you’ve done something amazing,” Underwood explains. “Here’s a person who saw that something was going to break and saw how it was going to break and devised a way to prevent it from breaking.”</p>
<p>That’s DevOps—or, in Google parlance, Site Reliability Engineering. As three words, it doesn’t sound like much. But it’s an enormously powerful idea. It has already produced Google. But particularly philosophical SREs like Underwood have even bigger ambitions. They envision a world where operations shift even further towards code. “We long for the day,” Underwood says, “when nobody runs anything.”</p>

			<a class="visually-hidden skip-to-text-link focusable bg-white" href="#start-of-content">Go Back to Top. Skip To: Start of Article.</a>

			
</div>
<br>[ad_2]
<br><a href="http://feeds.wired.com/c/35185/f/661370/s/4ec3ad08/sc/15/l/0L0Swired0N0C20A160C0A40Cgoogle0Eensures0Eservices0Ealmost0Enever0Ego0C/story01.htm">Source </a>