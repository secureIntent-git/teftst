---
ID: 1061
post_title: >
  Magistrate Orders Apple to Help FBI Hack
  San Bernardino Shooter’s Phone
author: Staff Writer
post_date: 2016-02-17 05:58:16
post_excerpt: ""
layout: post
permalink: >
  https://www.whenitson.com/magistrate-orders-apple-to-help-fbi-hack-san-bernardino-shooters-phone/
published: true
original_cats:
  - >
    terrorism,apple,privacy,Threat
    Level,encryption,Security,San
    Bernardino,FBI
original_title:
  - >
    Magistrate Orders Apple to Help FBI Hack
    San Bernardino Shooter’s Phone
original_link:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4da3d119/sc/28/l/0L0Swired0N0C20A160C0A20Cmagistrate0Eorders0Eapple0Eto0Ehelp0Efbi0Ehack0Ephone0Eof0Esan0Ebernardino0Eshooter0C/story01.htm
canonical_url:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4da3d119/sc/28/l/0L0Swired0N0C20A160C0A20Cmagistrate0Eorders0Eapple0Eto0Ehelp0Efbi0Ehack0Ephone0Eof0Esan0Ebernardino0Eshooter0C/story01.htm
---
 [ad_1]
<br><div id=""><p>A California magistrate has ordered Apple to help authorities hack a cell phone belonging to one of the shooters in the San Bernardino attack last year.</p>
<p>In an ironic twist, however, the FBI didn’t ask the court to order Apple to unlock the phone, but merely to help the FBI in its bruteforce attempts to unlock the device on its own.</p>
<p>Magistrate Sheri Pym, in the US District Court of Central California, ordered the tech giant to provide the FBI with software designed to defeat a self-destruct mechanism on the iPhone, according to the Associated Press, which <a href="http://bigstory.ap.org/article/145860f91b854a709c1a47190563c86e/judge-apple-must-help-us-hack-san-bernardino-killers-phone">first reported the news</a>. The self-destruct mechanism automatically erases data on a phone after ten failed password attempts, or rather erases a key that could be used to decrypt that data.</p>
<p>This would allow FBI agents to attempt to open the phone using multiple password tries—a method known as bruteforcing—without worrying that the data will be inaccessible to them forever.</p>
<p>According to the <a href="https://assets.documentcloud.org/documents/2714001/SB-Shooter-Order-Compelling-Apple-Asst-iPhone.pdf">court order</a> (.pdf), the phone in question is an iPhone 5c, with the iOS9 version of software running on it.</p>
<p>“Apple’s reasonable technical assistance shall accomplish the following three important functions,” the document notes. “It will bypass or disable the auto-erase function whether or not it has been enabled; it will enable the FBI to submit passcodes to the subject device for testing electronically via the physical device port, Bluetooth, Wi-Fi or other protocol available on the subject device and it will ensure that when the FBI submits passcodes to the subject device, software running on the device will not purposefully introduce any additional delay between the passcode attempts beyond what is incurred by Apple hardware.”</p>
<p>The magistrate allowed for the possibility that a solution for doing this might not be viable and asked Apple to respond if that’s the case.</p>
<p>The FBI has been saying for months that it is <a href="http://www.wired.com/2016/01/proposed-state-bans-on-phone-encryption-make-zero-sense/">losing its ability to collect crucial intelligence</a> because companies like Apple refuse to provide law enforcement with a backdoor to access phone data via a court order.</p>
<p>But the FBI’s request in this case marks an intriguing twist to that because it shows that the FBI is confident in its ability to bruteforce a locked and encrypted phone, given the ability to try an unlimited number of password guesses.</p>
<p>“Now here’s a case where [the FBI] really want[s] to get into the phone and they’re suddenly able to become much more creative than they have let on,” says Matt Blaze, a cryptographer and computer science professor at the University of Pennsylvania. “It is well-known that people tend to use weak, brute-foreable passwords. And I suspect that the FBI is betting that this [case] is no exception. It’s entirely possible that the FBI’s strategy [for unlocking the device] is very likely to be quite successful.”</p>
<p>Oddly, in its <a href="http://www.wired.com/wp-content/uploads/2016/02/SB-shooter-MOTION-seeking-asst-iPhone.pdf">40-page motion to the court</a> (.pdf), the government seems to indicate that it hasn’t attempted any password guess yet to unlock the phone, despite statements in the media by the FBI that it has tried everything possible to unlock the phone over the last two months.</p>
<p>In their motion, authorities write that Apple has designed its iPhone software to invoke time delays after repeated, unsuccessful password attempts. “This means that after each failed passcode entry, the user must wait a period of time before another attempt can be made, up to a 1-hour delay after the ninth failed attempt….”</p>
<p>The government asked the court to order Apple to provide it with a unique custom signed iPhone software that it can be loaded only onto the iPhone in question and run from the RAM, so that it would not change the operating system or any of the user data. This program would allow the FBI to test multiple passcodes on the device without triggering the auto-delete function, without having to type the passwords manually onto the touchscreen and without having the iPhone introduce excessive delays between password attempts.</p>
<p>It’s unclear if Apple has an existing software tool capable of defeating the auto-delete function. Blaze says such a tool would likely need to disable the count limit on the device that tallies each password attempt. But if this is the case, this presumably would be a security failure, since hackers might be able to design their own software to defeat or disable the counter.</p>
<p>Matthew Green, a cryptographer and professor at Johns Hopkins University, says that Apple and the FBI might indeed be able to defeat the count limit, but doubts they would be able to defeat the 80-millisecond delay the government writes about in its motion, which Apple has built into its software <a href="http://blog.cryptographyengineering.com/2014/10/why-cant-apple-decrypt-your-iphone.html">to thwart bruteforcing password attempts</a>. At least it would not be able to defeat the delay if the password on the device is strong, he says.</p>
<p>“[T]he bottom line is that Apple can comply with this order and test passcodes on the phone,” he told WIRED. “But it will take 80 milliseconds per test. Do the math on that. With a bad password, it’ll take no time. With a strong one, it’ll take years.”</p>
<p>The phone in question is a county work phone used by Syed Rizwan Farook, who worked for the San Bernardino County Department of Public Health as a public health inspector. Farook and his wife Tashfeen Malik were responsible, authorities say, for killing 14 people and injuring another 22 who were attending a training event and holiday party last December 2. Both were later killed in a shootout with police.</p>
<p>Earlier this month, FBI Director James Comey told the Senate Intelligence Committee that after two months of trying, his agents had not been able to unlock a phone left behind by the San Bernardino attackers. “We still have one of those killers’ phones that we haven’t been able to open,” Comey told the committee. “It has been two months now and we are still working on it.” </p>
<p>It was the second case recently in which the FBI insisted that it was having trouble accessing data on a phone. In December, Comey said that his agency was unable to access messages that one of two gunmen in Texas had used to communicate with a suspected terrorist overseas. “We have no idea what he said, because those messages were encrypted,” he told the same committee at the time. </p>
<p>In the San Bernardino case, the government was careful to state that it wanted special software only for that specific phone. But civil liberties advocates say this is a slipper slope.</p>
<p>“What the court is essentially ordering Apple to do is custom-build malware to undermine its own product’s security features, and then cryptographically sign that software so the iPhone will trust it as coming from Apple,” says Kevin Bankston,  director of New America’s Open Technology Institute. “But If a court can legally compel Apple to do that, then it likely could also legally compel any other software provider to do the same, including compelling the secret installation of malware via automatic updates to your phone or laptop’s operating system or other software. In other words, this isn’t just about one iPhone, it’s about all of our software and all of our digital devices, and if this precedent gets set it will spell digital disaster for the trustworthiness of everyone’s computers and mobile phones.”</p>
<p><strong>Update 8:30pm:</strong> To add comment from Kevin Bankston.</p>

			<a class="visually-hidden skip-to-text-link focusable bg-white" href="#start-of-content">Go Back to Top. Skip To: Start of Article.</a>

			
</div>
<br>[ad_2]
<br><a href="http://feeds.wired.com/c/35185/f/661370/s/4da3d119/sc/28/l/0L0Swired0N0C20A160C0A20Cmagistrate0Eorders0Eapple0Eto0Ehelp0Efbi0Ehack0Ephone0Eof0Esan0Ebernardino0Eshooter0C/story01.htm">Source </a>