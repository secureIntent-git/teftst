---
ID: 1363
post_title: 'Hack Brief: Last Year’s IRS Hack Was Way Worse Than We Realized'
author: Staff Writer
post_date: 2016-02-27 11:14:09
post_excerpt: ""
layout: post
permalink: >
  https://www.whenitson.com/hack-brief-last-years-irs-hack-was-way-worse-than-we-realized/
published: true
original_cats:
  - >
    privacy,hack brief,irs,hacks,irs
    hack,Security
original_title:
  - 'Hack Brief: Last Year’s IRS Hack Was Way Worse Than We Realized'
original_link:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4de23fc9/sc/13/l/0L0Swired0N0C20A160C0A20Cirs0Ehack0E70A0A0A0A0A0Eaccounts0C/story01.htm
canonical_url:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4de23fc9/sc/13/l/0L0Swired0N0C20A160C0A20Cirs0Ehack0E70A0A0A0A0A0Eaccounts0C/story01.htm
---
 [ad_1]
<br><div id=""><p>The Apple ecosystem is well known <a href="http://www.wired.com/2015/08/secure-way-communicate-ipod-touch/"><span class="s2">for very rarely</span></a> letting any dodgy apps enter it because of the company’s stringent security checks.</p>
<p>But recently, nearly two dozen malicious pieces of software managed to get hosted on the App Store, and subsequently downloaded by Chinese users. This is because attackers found an unorthodox route to exploit: they targeted some versions of the software used by developers to makes apps for iOS and OS X in the first place.</p>
<h3>The Hack</h3>
<p>The malware was first highlighted by Chinese developers on Weibo, and was then analyzed by researchers <a href="http://drops.wooyun.org/news/8864"><span class="s3">from Alibaba</span></a>. Security company Palo Alto Networks then <a href="http://researchcenter.paloaltonetworks.com/2015/09/novel-malware-xcodeghost-modifies-xcode-infects-apple-ios-apps-and-hits-app-store/"><span class="s3">verified the results</span></a>.</p>
<p>The hack all hinges around Xcode, a tool used to create iOS and OS X apps. Typically, Xcode is <a href="https://developer.apple.com/xcode/download/"><span class="s2">downloaded directly</span></a> from Apple for free. However, it is possible to get Xcode from other sources too, such as developer forums. Some versions of Xcode found on Baidu Yunpan, a Chinese file-sharing service, come packaged with extra lines of code. The Alibaba researchers have dubbed these malicious variants “XcodeGhost.” </p>
<p>Apps constructed with XcodeGhost code will collect a bunch of information about a customer’s device once the app has been downloaded. The data siphoned includes the current time, the name of the device, and the network type—none of which is anything a hacker could really use against you.</p>
<p>One of the apps that passed Apple’s security checks was NetEase Cloud Music, which, according to a screenshot provided by Palo Alto Networks, has nearly 500 ratings, averaging out at four and a half stars. Claud Xiao, a senior malware researcher from Palo Alto Networks, tells WIRED in an email the company had verified over 20 apps that were infected.</p>
<p>“Some of them are very popular and have tens of millions of installations,” Xiao writes.</p>
<h3>Who’s Affected?</h3>
<p>The iOS users who downloaded these apps, first of all. However, the apps analyzed were reportedly only from the Chinese App Store, so it doesn’t look like customers from other areas of the world need to worry.</p>
<p>Also, any developers who obtained their copy of Xcode from an unofficial source could be affected, as there is a chance their products are not totally above board. XcodeGhost could also affect developers <a href="https://developer.apple.com/programs/enterprise/"><span class="s2">creating enterprise apps</span></a>. These are apps made by companies specifically for their own employees’ devices, so they don’t have to go through any sort of Apple security check. However, “that’s a pretty obscure attack,” Charlie Miller, a <a href="http://www.wired.com/2015/08/uber-hires-hackers-wirelessly-hijacked-jeep/"><span class="s2">security researcher at Uber</span></a> who got his own malicious software onto the A<a href="http://apple.slashdot.org/story/11/11/07/2029219/charlie-miller-circumvents-code-signing-for-ios-apps"><span class="s2">pp Store in 2011</span></a>, tells WIRED in a phone interview. </p>
<h3>How Severe Is This?</h3>
<p>The malware in the App Store itself is not concerning, but there’s a broader issue here: the way in which it got past Apple’s screening process in the first place.</p>
<p>“You might completely trust the app developer, and that developer might be completely trustworthy, but this is a case where the app wasn’t,” Miller said. That, and the fact that software made from a tampered version of Xcode found its way onto the App Store, should give developers pause.</p>
<p>Apple did not immediately return a request for comment.</p>
<p>But what about consumers, and the people who downloaded the malicious apps? They should be only slightly concerned. “I wouldn’t worry too much,” Miller says. The apps that did get through didn’t seem to do any really nasty stuff. “If you made it really, obviously bad, probably [Apple] would catch it,” Miller says. </p>
<p>The bottom line for customers is, if you’ve downloaded one of these dodgy apps, delete it, and keep up with reports of other ones slipping through. What should developers do to protect their own apps and their customers? </p>
<p>“The moral of the story is: don’t download random crap from Chinese sites,” Miller says. </p>
							<a class="visually-hidden skip-to-text-link focusable bg-white" href="#start-of-content">Go Back to Top. Skip To: Start of Article.</a>
						</div>
<br>[ad_2]
<br><a href="http://feeds.wired.com/c/35185/f/661370/s/4de23fc9/sc/13/l/0L0Swired0N0C20A160C0A20Cirs0Ehack0E70A0A0A0A0A0Eaccounts0C/story01.htm">Source </a>