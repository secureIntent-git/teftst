---
ID: 3410
post_title: 'Hacker Lexicon: Stingrays, the Spy Tool the Government Tried, and Failed, to Hide'
author: Staff Writer
post_date: 2016-05-07 06:32:07
post_excerpt: ""
layout: post
permalink: >
  https://www.whenitson.com/hacker-lexicon-stingrays-the-spy-tool-the-government-tried-and-failed-to-hide/
published: true
original_cats:
  - >
    Security,Threat Level,government
    surveillance,hacker
    lexicon,privacy,stingrays
original_title:
  - 'Hacker Lexicon: Stingrays, the Spy Tool the Government Tried, and Failed, to Hide'
original_link:
  - >
    http://www.wired.com/2016/05/hacker-lexicon-stingrays-spy-tool-government-tried-failed-hide/
canonical_url:
  - >
    http://www.wired.com/2016/05/hacker-lexicon-stingrays-spy-tool-government-tried-failed-hide/
---
 [ad_1]
<br><div id=""><p>Stingrays, a secretive law enforcement surveillance tool, are one of the most controversial technologies in the government’s spy kit. But prosecutors and law enforcement agencies around the country have exerted such great effort to deceive courts and the public about stingrays that learning how and when the technology is used is difficult. </p>
<p>This week, the government even went so far as to assert in <a href="https://www.wired.com/wp-content/uploads/2016/05/Stingray-no-deception.pdf">a court filing</a> (.pdf) that articles published by WIRED and other media outlets that expose the deception “are full of unproven claims by defense attorneys and advocates [and] are not proper proof of anything.”</p>
<p data-js="fader" class="pullquote carve fader">
	TL;DR: Stingrays impersonate a legitimate cell phone tower in order to trick mobile devices into connecting to them and revealing information about their user's location.	<span class="attribution"/>
</p>

<p>So what do we know? “Stingray” is the generic commercial term for a device otherwise known as an IMSI catcher. The stingray impersonates a legitimate cell tower to trick nearby mobile phones and other wireless communication devices, like air cards, into connecting to them and revealing their international mobile subscriber identity (IMSI) number. More importantly, though, the device also collects information that can point to a mobile device’s location.</p>
<p>By moving the stingray around a geographical area and gathering a wireless device’s signal strength from various locations in a neighborhood, authorities can pinpoint where the device is being used with more precision than with data obtained from a mobile network provider’s fixed tower location.</p>
<p>Although use of the spy technology goes back at least 20 years—the FBI used a primitive version of a stingray to <a href="http://archive.wired.com/wired/archive/4.02/catching.html">track former hacker Kevin Mitnick in 1994</a>—their use of it has grown in the last decade as mobile phones and devices have become ubiquitous. Today, they’re used by the military and CIA in conflict zones—to prevent adversaries from using a mobile phone to detonate roadside bombs, for example—as well as domestically by federal agencies like the FBI, DEA and US Marshals Service, and by local law enforcement agencies.</p>
<p>Stingrays have the ability to also capture call record data—such as the numbers being dialed from a phone—and some also have the ability to <a href="https://www.wired.com/2015/10/stingray-government-spy-tools-can-record-calls-new-documents-confirm/">record the content of phone calls</a>, as well as <a href="https://www.wired.com/2011/10/datong-surveillance/">jam phones</a> to prevent them from being used. Domestic law enforcement agencies in the US, however, insist that the model of stingrays they use don’t collect the contents of communications.</p>
<p>The use of stingrays is highly controversial, in part because the devices don’t just hook targeted phones—they entice any mobile phone or device in their vicinity to connect to them, as long as the phones are using the same cellular network as the targeted phone. Stingrays can also <a href="http://www.wired.com/2015/03/feds-admit-stingrays-can-disrupt-cell-service-bystanders/">disrupt cellular voice and text service for any device</a> that connects to them, since the devices are not connecting to a legitimate cell tower that will transmit their communication.</p>
<p>Some rogue towers will also attempt to intercept encrypted mobile communication by forcing a phone to downgrade from a 3G or 4G network connection to a 2G network—a less secure network that doesn’t authenticate cell towers to the phone and contains vulnerabilities that make it easier to decrypt secure communication. The IMSI catchers jam 3G and 4G signals to force the phone to use the less secure 2G network.</p>
<p>And stingrays aren’t cheap. One device from the Harris Corporation, which sells a brand of IMSI catcher actually named Stingray, can cost more than $50,000. But this doesn’t mean stingrays are beyond the reach of anyone but resource-rich law enforcement and intelligence agencies. In 2010 at the Def Con hacker conference in Las Vegas, a security researcher <a href="http://www.wired.com/2010/07/intercepting-cell-phone-calls/">crafted a low-cost, home-brewed stingray</a> for just $1,500 capable of intercepting traffic and disabling the encryption, showing just how easy it would be for anyone to use this technology to spy on calls. </p>
<p>Beyond the controversial ways stingray technology works, the secrecy and deception law enforcement agencies use to cloak their use of the devices is also troubling.</p>



<p>Law enforcement agencies around the country have routinely used the devices <a href="http://www.wired.com/2014/03/stingray/">without obtaining a warrant from judges</a>. In cases where they did obtain a warrant, they often deceived judges about the nature of the technology they planned to use. Instead of telling judges that they intended to use a stingray or cell site simulator, they have often <a href="http://www.wired.com/2015/04/ny-cops-used-stingray-spy-tool-46-times-without-warrant/">mischaracterized the technology</a>, describing it as a pen register device instead. Pen registers record the numbers dialed from a specific phone number and are not, for this reason, considered evasive. Because stingrays, however, are used to track the location and movement of a device, civil liberties groups consider them to be much more invasive. They can, for example, be used to track a device inside a private residence.</p>
<p>In some cases, law enforcement agents have also <a href="http://www.wired.com/2014/06/feds-told-cops-to-deceive-courts-about-stingray/">deceived defense attorneys about their use of stingrays</a>, saying they obtained knowledge of a suspect’s location from a “confidential source” rather than disclosing that the information was gleaned using a stingray.</p>
<p>Law enforcement agencies have also gone to great lengths to prevent the public from learning about their use of the technology. In Florida, for example, when the American Civil Liberties Union tried to obtain copies of documents from a local police department discussing their use of the technology, agents with the US Marshals Service <a href="http://www.wired.com/2014/06/feds-seize-stingray-documents/">swooped in at the last minute and seized the documents</a> to prevent police from releasing them. Law enforcement agencies claim that public information about the technology will prompt criminals to devise methods to subvert or bypass the surveillance tool. </p>
<p>Indeed, there are already apps and tools available to help detect rogue cell towers like stingrays. The German firm GSMK’s secure CryptoPhone, for example, has a firewall that can alert users to suspicious activity that may indicate when a <a href="http://www.wired.com/2014/09/cryptophone-firewall-identifies-rogue-cell-towers/">stingray has connected to their phone</a> or turned off the encryption their phone might be using. </p>
<p>Last year, the Justice Department announced a new policy for using stingrays that offers a little more transparency, but only a little. Under the policy, the FBI and any other federal agencies using stingrays will <a href="https://www.wired.com/2015/09/feds-need-warrant-spy-stingrays-now/">have to get a search warrant</a> before deploying them. The policy forces prosecutors and investigators not only to obtain a warrant, but also to disclose to judges that the specific technology they plan to use is a stingray—which prevents them from deceiving judges and defense attorneys about the surveillance method they plan to use. Agents using the device also have to delete all data a stingray collects “as soon as” it has located the device it’s tracking. </p>
<p>The only problem is that the new policy does not cover local and regional law enforcement, who also use stingrays to track suspects.</p>
<p>That may change, however: A bill introduced last year by Rep. Jason Chaffetz (R-Utah) hopes to fix that loophole. The Cell-Site Simulator Act of 2015, also known as the Stingray Privacy Act, would <a href="https://www.wired.com/2015/11/new-bill-would-force-cops-to-get-warrants-before-spying-with-stingrays/">force state and local law enforcement to obtain a warrant</a> as well.</p>

			<a class="visually-hidden skip-to-text-link focusable bg-white" href="#start-of-content">Go Back to Top. Skip To: Start of Article.</a>

			
</div>
<br>[ad_2]
<br><a href="http://www.wired.com/2016/05/hacker-lexicon-stingrays-spy-tool-government-tried-failed-hide/">Source </a>