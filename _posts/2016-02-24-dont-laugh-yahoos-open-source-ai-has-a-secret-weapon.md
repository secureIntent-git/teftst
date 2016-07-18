---
ID: 1285
post_title: 'Don’t Laugh: Yahoo’s Open Source AI Has a Secret Weapon'
author: Staff Writer
post_date: 2016-02-24 21:52:10
post_excerpt: ""
layout: post
permalink: >
  https://www.whenitson.com/dont-laugh-yahoos-open-source-ai-has-a-secret-weapon/
published: true
original_cats:
  - >
    Yahoo,Artificial Intelligence,big
    data,ai,open-source,Spark,deep
    learning,Business
original_title:
  - 'Don’t Laugh: Yahoo’s Open Source AI Has a Secret Weapon'
original_link:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4dd407f5/sc/13/l/0L0Swired0N0C20A160C0A20Cdont0Elaugh0Eyahoos0Eopen0Esource0Eai0Esecret0Eweapon0C/story01.htm
canonical_url:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4dd407f5/sc/13/l/0L0Swired0N0C20A160C0A20Cdont0Elaugh0Eyahoos0Eopen0Esource0Eai0Esecret0Eweapon0C/story01.htm
---
 [ad_1]
<br><div id=""><div id="small-art" data-share="">
				<figure attachment_1979523="" class="carve wp-caption portrait alignnone  relative" data-js=""><a href="http://www.wired.com/wp-content/uploads/2016/02/GettyImages-501867023.jpg"><img data-pin-description="Don’t Laugh: Yahoo’s Open Source AI Has a Secret Weapon" src="http://www.whenitson.com/wp-content/uploads/2016/02/Dont-Laugh-Yahoos-Open-Source-AI-Has-a-Secret-Weapon.jpg" alt="GettyImages-501867023.jpg" width="853" height="1024" class="size-large wp-image-1979523"/></a><figcaption class="wp-caption-text link-underline"><span class="credit link-underline-sm"><span aria-hidden="true" class="ui ui-photo inline-block ui-credit relative opacity-5 marg-r-micro"/> Getty Images</span></figcaption></figure></div>

			<p>Yet another tech giant is sharing its artificial intelligence know-how with the world. Today Yahoo published the source code to its CaffeOnSpark AI engine so that anyone from academic researchers to big corporations can use or modify it. </p>
<p>Yahoo may not be known as much for its technological prowess these days. But it did incubate Hadoop, an open source, wildly popular data crunching platform used by Facebook, Twitter and scores of other companies. And when it comes to AI, it has a unique asset. When training artificial intelligence systems, the data matters as much as the algorithms. And Yahoo has one of the more interesting data sets around in the form of Yahoo-owned photo site Flickr.</p>
<p data-js="fader" class="pullquote carve fader">
	When training artificial intelligence systems, the data matters as much as the algorithms.	<span class="attribution"/>
</p>

<p>Like so many other new open source AI project, CaffeOnSpark is based on deep learning, a branch of artificial intelligence particularly useful in helping machines recognize human speech, or the contents of a photo or video. Yahoo, for example, uses it to improve search results on Flickr by determining the contents of different photos. Instead of relying on the descriptions and keywords entered by the people who upload photos to the site, Yahoo teaches its computers to recognize certain characteristics of a photo, such as specific colors or even objects and animals. </p>
<p>In recent months Google has open sourced its deep learning framework <a href="http://www.wired.com/2015/11/google-open-sources-its-artificial-intelligence-engine/">TensorFlow</a>, Microsoft opened up its similar framework <a href="http://www.wired.com/2016/01/microsoft-tries-to-one-up-google-in-the-open-source-ai-race/">CNTK</a>, Facebook shared its <a href="http://www.wired.com/2015/12/facebook-open-source-ai-big-sur/">AI hardware designs</a>, and Chinese search giant Baidu unveiled its <a href="http://research.baidu.com/warp-ctc/">deep learning training software</a><a/>.</p>



<p>Each of these pieces of open source technology scratches a different itch. For Yahoo, it’s the desire to run deep learning processes on existing systems without the need to move data from one place to another. Training a deep learning system to recognize images requires huge amounts of data, Yahoo vice president of architecture Andy Feng explains. You feed an algorithm as many examples as you can of, say, a cat, and eventually the machine will “learn” the common features of cats and and be able to tell photos that include cats from those that don’t.</p>
<p>Flickr hosts billions of photos, a plentiful selection of images with which to train an AI. But the team didn’t want to have to copy all those images from the primary Flickr servers to a new cluster of servers running deep learning software. So they invented a way to run deep learning software on their existing infrastructure.</p>
<p>CaffeOnSpark, as the name suggests, combines two existing technologies: the popular deep learning framework <a href="http://caffe.berkeleyvision.org/">Caffe</a> and the up-and-coming data-crunching system <a href="http://www.wired.com/2013/06/yahoo-amazon-amplab-spark/all/">Spark</a> that can run on top of the even more popular big data platform Hadoop. What Yahoo did was simply create a way to run Caffee atop Spark clusters. It can be run either on Spark alone or atop Hadoop. Besides making it easy for AI developers to use familiar tools and avoid moving data around, Feng says CaffeOnSpark also makes it relatively easy to distribute deep learning processes across multiple servers, something that the open source version of Google’s TensorFlow can’t yet do.</p>
<p>Feng says a number of companies asking Yahoo to open source CaffeOnSpark last year after the team published a <a href="http://yahoohadoop.tumblr.com/post/129872361846/large-scale-distributed-deep-learning-on-hadoop">blog post</a> about the software. It turns out a lot of organizations having data sitting on server clusters that they don’t want to move it around.</p>

			<a class="visually-hidden skip-to-text-link focusable bg-white" href="#start-of-content">Go Back to Top. Skip To: Start of Article.</a>

			
</div>
<br>[ad_2]
<br><a href="http://feeds.wired.com/c/35185/f/661370/s/4dd407f5/sc/13/l/0L0Swired0N0C20A160C0A20Cdont0Elaugh0Eyahoos0Eopen0Esource0Eai0Esecret0Eweapon0C/story01.htm">Source </a>