---
ID: 1246
post_title: >
  Flaws in Wireless Mice and Keyboards Let
  Hackers Type on Your PC
author: Staff Writer
post_date: 2016-02-23 15:08:05
post_excerpt: ""
layout: post
permalink: >
  https://www.whenitson.com/flaws-in-wireless-mice-and-keyboards-let-hackers-type-on-your-pc/
published: true
original_cats:
  - >
    Amazon,Threat
    Level,dongle,mousejack,wifi,microsoft,Bluetooth,Dell,gigbyte,hp,bastille,Lenovo,logitech,Security,RSA,mousejacking
original_title:
  - >
    Flaws in Wireless Mice and Keyboards Let
    Hackers Type on Your PC
original_link:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4dcaf9bc/sc/28/l/0L0Swired0N0C20A160C0A20Cflaws0Ein0Ewireless0Emice0Eand0Ekeyboards0Elet0Ehackers0Etype0Eon0Eyour0Epc0C/story01.htm
canonical_url:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4dcaf9bc/sc/28/l/0L0Swired0N0C20A160C0A20Cflaws0Ein0Ewireless0Emice0Eand0Ekeyboards0Elet0Ehackers0Etype0Eon0Eyour0Epc0C/story01.htm
dsq_thread_id:
  - "4604792134"
---
 [ad_1]
<br><div id=""><p>That tiny dongle plugged into your USB port and paired with your wireless keyboard or mouse isn’t as monogamous as it pretends to be. For millions of cheap peripherals, those innocent-looking radio receivers may be carrying on a sly, long distance relationship—letting an antenna-wielding intruder silently type malicious commands on your PC.</p>
<p>That’s a new warning from researchers at the Internet of things security firm Bastille, who released an advisory today that seven different companies’ wireless keyboards and mice are vulnerable to an exploit they’ve dubbed “mousejacking.” The attack—which affects a broad collection of devices sold by Logitech, Dell, Microsoft, HP, Amazon, Gigabyte and Lenovo—lets an interloper inject mouse movements or keystrokes at a rate of a thousand words per minute from an nearby antenna, even when the target device is designed to encrypt and authenticate its communications with a paired computer.</p>
<p>“With about fifteen lines of code, you can take over a computer more than a hundred yards away,” says Chris Rouland, Bastille’s CEO, who previously founded the hacking firm Endgame, a US government contractor. In their tests, Rouland and Bastille researcher Marc Newlin used a <a rel="nofollow" href="http://www.amazon.com/dp/B014O8D7D0/?tag=w050b-20" target="_blank">$12 Geeetech Crazyradio USB radio dongle</a> attached to a laptop running their exploit code to pair with the victim devices. They tested as far as that hundred-yard range, though they found that the attack was more reliable with a more powerful <a rel="nofollow" href="http://www.amazon.com/dp/B00KL6X9M4/?tag=w050b-20" target="_blank">Yagi antenna</a> and believe it could likely be extended further. They also built a radio-enabled Nintendo controller capable of running their attack software, which they plan to show off at the RSA conference in San Francisco next week. Rouland points out that the exploit, which affects devices that use a little-studied proprietary radio protocol rather than Wi-Fi or Bluetooth, leaves even PCs that have been “airgapped”—isolated from the Internet—vulnerable if someone has plugged in a wireless keyboard dongle.</p>
<p>“We can compromise an airgapped network, going in through a different frequency protocol, directly to the USB port,” he says.</p>
<h3>How It Works</h3>
<p>Bastille’s mousejack attack doesn’t take advantage of one single vulnerability, but instead a collection of distinct problems in the firmware of wireless devices that use chips sold by the Norwegian firm Nordic Semiconductor. Nordic chips are capable of encryption. But unlike standard Bluetooth chips, the Norwegian firm’s cheap, low-power shortrange radio communications chips require that vendors write their own firmware to implement that encryption and secure the connection between computers and peripheral devices. The result, Bastille’s researchers say, is that many of the affected companies failed to take advantage of Nordic’s encryption option, allowing the dongles that receive those communications to accept keystrokes from another device using the same radio protocol. Most of the vulnerable keyboards <em>did</em> encrypt their communications, the researchers say, but didn’t properly authenticate communicating devices; they would still allow another rogue device to inject unencrypted keystrokes over the same connection. “It’s like having an expensive deadbolt and leaving it unlocked,” says Rouland.</p>
<p data-js="fader" class="pullquote carve fader">
	I don't think people even understand that there’s firmware in the dongle connected to their mouse.	<span class="attribution">Chris Rouland</span>
</p>

<p>The Bastille researchers claim that “more than a billion” devices are affected in total. They back up that questionable number by pointing to a 2008 press release from Logitech touting the <a href="http://www.logitech.com/en-us/press/press-releases/5388" target="_blank">shipment of its billionth mouse</a>, but couldn’t point to a more recent count or one that distinguishes between wireless and wired devices. Given the number of companies whose products Bastille successfully attacked, however, the count of vulnerable mice and keyboards is likely high, possibly in the millions; Rouland says that in Bastille’s tests, they were able to spot vulnerable wireless device dongles in most office buildings they targeted with their antennae. “Once you start looking for that little dongle, you’ll see it everywhere,” Rouland says.</p>
<p>Injecting keystrokes on a target computer, of course, isn’t in itself a full compromise of the machine. The hacker would only have the same privileges as the person using the computer and wouldn’t necessarily be able to type his or her passwords. Rouland argues that the attack could quickly be used to download malware and take full remote control of a PC. But the computer would have to already be unlocked, a caveat that would likely require the attacker to be able to see his or her target’s screen.</p>
<figure attachment_1978334="" class="wp-caption landscape alignnone fader relative" data-js="fader"><a href="http://www.wired.com/wp-content/uploads/2016/02/IMG_5727-1.jpg"><img class="wp-image-1978334 size-large" src="http://www.whenitson.com/wp-content/uploads/2016/02/Flaws-in-Wireless-Mice-and-Keyboards-Let-Hackers-Type-on-Your-PC.jpg" alt="IMG_5727-1.jpg" width="1024" height="682"/></a><figcaption class="wp-caption-text link-underline">The $12 Crazyradio USB radio and antenna the security researchers used to hack the wireless keyboards and mice. <span class="credit link-underline-sm"><span aria-hidden="true" class="ui ui ui-photo inline-block ui-credit relative opacity-5 marg-r-micro"/> Bastille</span></figcaption></figure><h3>What Manufacturers (And You) Can Do</h3>
<p>When WIRED reached out to the affected vendors, some downplayed the severity of the mousejacking attack. “The vulnerability would be complex to replicate and would require physical proximity to the target,” a Logitech spokesperson wrote in a statement. “It is therefore a difficult and unlikely path of attack.” Lenovo wrote in a statement that the severity of the attack is “low” and claims without explanation that its range would be only 10 meters. Bastille’s researchers, who had initially range-tested their attack only on Logitech devices, responded to Lenovo’s claim by trying the long-range mousejacking attack on Lenovo devices, too, and say they were able to inject keystrokes from 180 meters away.<sup>1</sup></p>
<p>But Dell, Logitech, Lenovo and Microsoft all acknowledged the vulnerability; Logitech says that with Bastille’s help it’s developed a firmware update for affected devices. Some Dell wireless keyboards use the same firmware, and the company tells WIRED those keyboards receive the Logitech update, too. Lenovo’s statement, on the other hand, admits it can’t update its vulnerable devices and instead will offer to replace them for any customer who asks. Microsoft’s statement notes only that the company “will proactively update impacted devices as soon as possible.” Amazon, Gigabyte, and HP have yet to respond to WIRED’s request for comment.</p>
<p data-js="fader" class="pullquote carve fader">
	Now someone has finally taken a look and found that virtually all of (these devices) are vulnerable. That’s pretty scary.	<span class="attribution">Samy Kamkar</span>
</p>

<p>The Bastille researchers aren’t the first to warn of the dangers of wireless keyboards and mice. Early last year, independent hacker Samy Kamkar released the code and specs for <a href="http://samy.pl/keysweeper/" target="_blank">KeySweeper</a>, a fake USB charger that can both eavesdrop on and inject keystrokes from certain Microsoft wireless keyboards. Kamkar’s device worked only on unencrypted keyboards, however. Bastille researcher Marc Newlin painstakingly tested this mousejacking attack on many more brands and models of devices. “It’s a bit of a wakeup call when it comes to the implementations of these protocols that are entirely proprietary and that no one has looked at before,” says Kamkar of Bastille’s research. “Now someone has finally taken a look and found that virtually all of them are vulnerable. That’s pretty scary.”</p>
<p>Unlike Kamkar in the case of his KeySweeper attack, however, Bastille has opted not to release its code for fear that mousejacking could be used for malicious purposes against unpatched—or unpatchable—devices. “This vulnerability will be out for 10 years,” estimated Rouland. “When was the last time people updated their router’s firmware? I don’t think people even understand that there’s firmware in the dongle connected to their mouse.”</p>
<p>But even without a public exploit from Bastille, other hackers could soon reverse engineer the attack and release it publicly. That means you should update or replace any vulnerable devices you use ASAP. Or better, says Kamkar, you should switch to more fully tested Bluetooth mice and keyboards. Or the safest fix of all, he suggests: give up on wireless peripherals altogether. “If you can go wired,” says Kamkar, “Go wired.”</p>
<p><sup>1</sup><em>Updated 2/23/2016 10am EST following Bastille’s further testing of their attack on Lenovo devices.</em></p>

			<a class="visually-hidden skip-to-text-link focusable bg-white" href="#start-of-content">Go Back to Top. Skip To: Start of Article.</a>

			
</div>
<br>[ad_2]
<br><a href="http://feeds.wired.com/c/35185/f/661370/s/4dcaf9bc/sc/28/l/0L0Swired0N0C20A160C0A20Cflaws0Ein0Ewireless0Emice0Eand0Ekeyboards0Elet0Ehackers0Etype0Eon0Eyour0Epc0C/story01.htm">Source </a>