---
ID: 4905
post_title: >
  So Hey You Should Stop Using Texts for
  Two-Factor Authentication
author: Staff Writer
post_date: 2016-06-26 15:04:09
post_excerpt: ""
layout: post
permalink: >
  https://www.whenitson.com/so-hey-you-should-stop-using-texts-for-two-factor-authentication/
published: true
original_cats:
  - >
    Security,Threat Level,2fa,security,sim
    swap,sms,two factor,two-factor
    authentication
original_title:
  - >
    So Hey You Should Stop Using Texts for
    Two-Factor Authentication
original_link:
  - >
    https://www.wired.com/2016/06/hey-stop-using-texts-two-factor-authentication/
canonical_url:
  - >
    https://www.wired.com/2016/06/hey-stop-using-texts-two-factor-authentication/
---
 [ad_1]
<br><div id=""><p>Since two-factor authentication became the norm for web services that care about securing your accounts, it’s started to feel like a security blanket, an extra layer keeping your data safe no matter whether your password is as strong as 8$&amp;]$@I)9[P&amp;4^s or as dumb as <a href="http://www.wired.co.uk/article/mark-zuckerberg-hacked-password-released" target="_blank">dadada</a>. But a two-factor setup—which for most users requires a temporary code generated on, or sent to, your phone in addition to a password—isn’t an invincibility spell. Especially if that second factor is delivered via text message.</p>
<p>The last few months have demonstrated that SMS text messages are often the weakest link in two-step logins: Attacks on political activists in Iran, Russia, and even here in the US have shown that determined hackers can sometimes hijack the SMS messages meant to keep you safe. Whenever possible, it’s worth taking a minute to switch to a better system, like an authentication smartphone app or a physical token that generates one-time codes. And for services like Twitter that <em>only</em> offer text messages as a second factor, it’s time to wake up, smell the targeted attacks, and give users better options.</p>
<p>“SMS is just not the best way to do this,” says security researcher and forensics expert Jonathan Zdziarski. “It’s depending on your mobile phone as a means of authentication [in a way] that can be socially engineered out of your control.”</p>
<p>That kind of social engineering is more than hypothetical. Earlier this month, Black Lives Matter activist DeRay McKesson <a href="https://www.wired.com/2016/06/deray-twitter-hack-2-factor-isnt-enough/" target="_blank">found that his Twitter account was hacked</a> to tweet pro-Donald Trump messages, despite having two-factor authentication in place. The hackers, as he tells it, had called up Verizon, impersonated him, and convinced the company to redirect his text messages to a different SIM card, intercepting his one-time login codes. And <a href="https://www.fredericjacobs.com/blog/2016/01/14/sms-login/" target="_blank">activists in Iran</a> <a href="https://www.fredericjacobs.com/blog/2016/04/30/more-on-sms-logins/" target="_blank">and in Russia</a> both recently found that their Telegram accounts were being hacked, likely by state-owned telecom companies helping those authoritarian governments to hijack the SMS messages Telegram uses to log users in. </p>
<p>In fact, one doesn’t have to be a public figure to become a target. As password security expect Lorrie Cranor <a href="http://www.wired.com/2016/06/even-ftcs-lead-technologist-can-get-hacked/" target="_blank">suffered a related hack</a>, she noted that these “SIM swap” attacks have grown prevalent enough to prompt New York State to <a href="https://www.dos.ny.gov/consumerprotection/scams/att-sim.html" target="_blank">issue an official warning</a>. </p>
<p>Adding a layer of SMS-based verification to your login process is certainly better than relying on a password alone. But Zdziarski goes so far as to argue that two-factor authentication using SMS text messages isn’t technically two-factor at all. The idea of two-factor authentication, he points out, is to test someone’s identity based on something they know (like a password) and something they have (like their phone or another device.) Better tools like Google Authenticator or an RSA token prove that possession, by generating a unique code that matches one generated on a web service’s server. It’s a test that, thanks to some clever crypto tricks, doesn’t involve any communication between the two computers. That’s far more effective than sending a text message with a one-time code to someone’s phone. It’s less convenient, though, which may be why it’s also less commonplace.</p>
<p>“SMS has turned that ‘something you have’ into ‘something they sent you,'” says Zdziarski. “If that transaction is happening, it can be intercepted. And that means you’re potentially at some level of risk.”</p>
<p>Tactics like social-engineering or strong-arming the phone company to subvert two-factor comprise only a fraction of SMS vulnerabilities. Fake cell phone towers known as IMSI catchers or “stingrays” can intercept text messages, too. And the security community has <a href="https://www.wired.com/2016/04/the-critical-hole-at-the-heart-of-cell-phone-infrastructure/" target="_blank">recently been calling attention to weaknesses in SS7</a>, the protocol that allows telecom networks to communicate with each other. Hackers can exploit SS7 to spoof a change to a user’s phone number, intercepting their calls or text messages. “Any network can tell any other network ‘your subscriber’s here now,’ and until your phone says otherwise, every call and text is diverted to this other network,” says Karsten Nohl, the chief scientist at Security Research Labs, who recently demonstrated the attack for 60 Minutes. “If there’s an attacker, they get all your text messages. it’s completely trust-based…It’s so simple it’s almost embarrassing to call it a hack.”</p>
<p>Those attacks aren’t exactly easy to pull off, and likely require the attacker to figure out the user’s cell phone number in addition to the password that they’ve stolen, guessed, or reused after being compromised in a data breach from another hacked service. But for anyone who might be a target of sophisticated hackers, all of those techniques mean SMS should be avoided when possible for anything login-related.</p>
<p>Luckily, plenty of services offer better options. Google last week <a href="http://lifehacker.com/google-prompt-lets-you-use-two-factor-authentication-wi-1782413235" target="_blank">launched Google Prompt</a>, a service that sends a second-factor login prompt directly from its servers to Android phones or to the Google Search app for iOS. But even more secure still are systems that don’t require any message to be sent at all. Apps like Google Authenticator and tokens like those sold by RSA generate one-time-password codes that change ever few seconds. Those same exact codes are generated on the servers run by services like Slack, WordPress, or Gmail, so that the user can cough up the code to prove their identity without it ever being sent over the internet. (The math behind that system is clever: When the user signs up for the service, the Google Authenticator app and the server both start with a seed value that’s transformed into a long, unique string of characters with a “hash”—a mathematical function that can’t be reversed. Then that string of characters is hashed again, and results are hashed again, repeating every few seconds. And only a few digits of those characters are displayed as the login code, so that no one who glances at a user’s phone can start their own hash chain.)</p>
<p>Unfortunately, some services like Twitter still only offer two-factor authentication via text message. But the embarrassment of high-profile hacks like DeRay McKesson’s account may have had some effect. Twitter tells WIRED in a statement that “we’re exploring additional ways to make sure your account stays secure.” In other words, Twitter, like other services that store your sensitive data, may soon be offering a second-factor option other than the rickety telephone line that SMS represents. And security-conscious users should take it.</p>

			<a class="visually-hidden skip-to-text-link focusable bg-white" href="#start-of-content">Go Back to Top. Skip To: Start of Article.</a>

			
</div>
<br>[ad_2]
<br><a href="https://www.wired.com/2016/06/hey-stop-using-texts-two-factor-authentication/">Source </a>