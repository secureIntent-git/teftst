---
ID: 2885
post_title: >
  You Want to Build an Empire Like
  Google’s? This Is Your OS
author: Staff Writer
post_date: 2016-04-19 08:34:04
post_excerpt: ""
layout: post
permalink: >
  https://www.whenitson.com/you-want-to-build-an-empire-like-googles-this-is-your-os/
published: true
original_cats:
  - >
    Business,Enterprise,airbnb,Containers,CoreOS,Docker,google,Google
    Kubernetes,Kubernetes,Mesos,twitter
original_title:
  - >
    You Want to Build an Empire Like
    Google’s? This Is Your OS
original_link:
  - >
    http://www.wired.com/2016/04/want-build-empire-like-googles-os/
canonical_url:
  - >
    http://www.wired.com/2016/04/want-build-empire-like-googles-os/
---
 [ad_1]
<br><div id=""><p>Google called it Borg, and for many years, it was among the company’s best-kept secrets.</p>
<p><a href="http://www.wired.com/2013/03/google-borg-twitter-mesos/" target="_blank">Borg ran just about everything within the company</a>, including Google Search, Gmail, Google Maps, Google Docs, and any other Google service you can think of—not to mention the private services you and I never see. Basically, it provided a way of parceling tasks across dozens, hundreds, even thousands of machines with extreme efficiency. A few years ago, uber Google engineer John Wilkes told me Borg was so efficient—so adept at finding a use for available processing power on each and every machine—that it had probably saved Google the cost of building another data center. And those things are expensive.</p>
<p>Even then, Borg remained veiled in secrecy. Wilkes wouldn’t even refer to it by name. But inside another big-name company, Twitter, Ben Hindman was recreating this sweeping software tool alongside several former Google engineers. They called it Mesos. Hindman started the project as a grad student at UC Berkeley, and after joining Twitter, he used it to rebuild the very foundation of the company’s microblogging service. Mesos was a little different from Borg—and Twitter a little smaller than Google—but Hindman’s creation served the same basic purpose, allowing Twitter to efficiently run software across a massive data center in much the same way you run software on a phone or laptop.</p>
<p>Now, Hindman hopes to bring this idea to every company on the planet. From the beginning, Mesos was an open source project, meaning anyone could use and modify the code, and after leaving Twitter, Hindman helped launch Mesosphere, a company that aims to help businesses embrace the project—in essence, helping them build a Borg of their own. Today, in an effort to advance this goal, Hindman and company open sourced other software tools that work in tandem with Mesos.</p>
<p>Collectively, all this software is called DC/OS, or data center operating system—which is kinda catchy. This, Hindman says, was the original vision for the company: to create an operating system that lets anyone run vast online services across a data center. But the decision to open source DC/OS also reflects—and is likely a response to—the rapid evolution of so many other tools that seek to do much the same thing. </p>
<h3>The Container Revolution</h3>
<p>The move comes amid an enormous revolution sweeping information technology, one in which big-name companies and startups alike aim to recreate Borg for the rest of the world. Alex Polvi, who runs one of these startups, CoreOS, describes the revolution with a hashtag: <a href="http://www.wired.com/2016/02/ibm-learns-to-stop-worrying-and-love-the-cloud-for-real/" target="_blank">#GIFEE</a>, or Google Infrastructure For Everyone Else—which is even catchier. In addition to Mesosphere and CoreOS, <a href="http://www.wired.com/2015/04/solomon-hykes/" target="_blank">a company called Docker is pushing this idea</a> alongside the biggest names in cloud computing: Amazon, Microsoft, and, yes, Google.</p>
<p>In the three years since Wilkes referred to Borg as “the system that will not be named”—a level of secrecy indicative of how Google treated the tech driving its data centers—the company has entered a period in which it not only freely discusses many of these technologies, but actively shares code. This is a way of driving the <a href="http://www.wired.com/2016/03/tech-exec-wants-cloud-googles-moneymaker/" target="_blank">use of its cloud computing services</a>, which are now enormously important to Google. In the summer of 2014, the company unveiled Kubernetes, its own open source effort to <a href="http://www.wired.com/2015/06/google-kubernetes-says-future-cloud-computing/" target="_blank">create a version of Borg others could use</a>. Now that Kubernetes is open source, it seems, Mesosphere must open source all of DC/OS. By itself, Mesos provides only part of what Kubernetes offers.</p>
<p>In any event, even Google believes in Google Infrastructure For Everyone Else. And it stands to reason, because Google and so many other companies have proven th benefits of the Borg idea, which involves <a href="http://www.wired.com/2014/06/eric-brewer-google-docker/" target="_blank">packaging software into tiny “containers”</a> that can run on any machine across a data center or, indeed, across multiple data centers. If you can do that, you can efficiency pack myriad containers onto each machine.</p>
<p>This may sound a bit like an older technology called <em>virtualization</em>, but tools like DC/OS and Kubernetes takes things much further. For one, they can run massive quantities of software far more efficiently than virtualization ever could. “The magic of the container world is that the computational overhead is far less than full virtualization,” says Mike Stoppelman, the senior vice president of engineering at Yelp, which now runs its operation at DC/OS. “Even today, moving around a 20 megabyte container is so much easier than moving a 100 megabyte virtual image … and the network traffic created by this stuff is an order of magnitude less.”</p>
<p>But this also is about improving the lives of software engineers. Any company that hits 50 to 100 engineers, Stoppelman says, almost <em>has to embrace</em> this kind of container architecture. It must break down its software into tiny pieces that can by run across myriad machines. Otherwise, things get too unwieldy. Tools like DC/OS and Kubernetes make it far easier to build that kind of distributed software. And the importance of this should not be underestimated. After all, software that runs across dozens or even hundreds of machines—think Google and Twitter and Apple Siri—drives the modern world.</p>
<h3>From Google to AirBnb to Yelp</h3>
<p>The container revolution is quite real. Hindman redesigned Twitter’s infrastructure alongside his old friend Florian Leibert, who helped bring the container idea to Airbnb. Now, they’re both at Mesosphere, where they’ve helped pushe the idea into countless other companies, including Yelp, Netflix, Autodesk, and Apple. This really is Google’s infrastructure spreading everywhere. Stoppelman, once a senior engineer at Google describes Yelp’s new infrastructure as “very similar to Borg.”</p>
<p>Stoppelman notes that Mesosphere developed an early lead in the new market, and Polvi says much the same thing. But Polvi also believes the market eventually will center on Kubernetes. His company offers an individual server operating system, CoreOS, that works with tools like Kubernetes, and he has worked closely with Google on the open source project. “I think things kinda converge on Kubernetes in due course,” Polvi says. “Kubernetes nailed the interface—the API—for how you talk to these distributed systems.”</p>
<p>That said, Mesophere’s DC/OS is clearly an effort to narrow any gap. It seeks to expand Mesos into more than just a technology for hardcore engineers, into software that any business can use.</p>
<h3>In the Clouds</h3>
<p>Companies are also using such tools atop cloud computing services. Yelp runs much of its infrastructure, for instance, on the Amazon cloud. And this is where things can get confusing. Cloud services rely on virtualization—they offer virtual machines where customers can run software without setting up physical machines—but containers still make sense when running atop virtual machines. You can still increase efficiency—if not quite as much—and more importantly, you can still <a href="http://www.wired.com/2014/06/eric-brewer-google-docker/" target="_blank">improve life for coders</a>.</p>
<p>One reason Mesosphere is opening sourcing DC/OS is that this makes it easier for companies to run the tool both atop outside cloud services and inside their own data centers. For instance, Microsoft (which is an investor in Mesophere) uses DC/OS to drive a kind of container service it offers atop its cloud, and now, if they so desire, business can their software atop both this service and a version of DC/OS running on their own machines. Google pushes the same idea. It offers Kubernetes as a cloud service, but since the tool is open source, you’re also free to use Kubernetes in your own data center. “That’s one of the great value propositions of open source,” says Mark Russinovich, the chief technology officer of Microsoft Azure. “People get this portability.”</p>
<h3>Windows, Here We Come</h3>
<p>Microsoft’s involvement is interesting because containers grew out of the open source Linux operating system, a rival to its own Windows OS. At Google, Borg drove thousands of machines loaded with Linux. The same goes for Twitter and Airbnb and Yelp. Containers were designed for Linux, and DC/OS only works with Linux machines.</p>
<p>Yes, it’s interesting that Microsoft is embracing a Linux technology, but that’s just how the company operates nowadays. Much as Google realized that the age of cloud computing means it must freely share its data center technologies, <a href="http://www.wired.com/2014/10/microsoft-ceo-satya-nadella-loves-steve-ballmer-despised/" target="_blank">Microsoft came to see it must embrace open source software atop its cloud</a>. But Redmond also is trying to recreate the container idea for use with its own Windows operating system.</p>
<p>Microsoft has already built a version of Windows that juggles containers—it uses this to run servers across its own online empire—and as Russinnovich notes, the company is working with Mesosphere to build a version of DC/OS that works with Windows. It really is Google Infrastructure for Everyone Else—including everyone who runs Microsoft software.</p>

			<a class="visually-hidden skip-to-text-link focusable bg-white" href="#start-of-content">Go Back to Top. Skip To: Start of Article.</a>

			
</div>
<br>[ad_2]
<br><a href="http://www.wired.com/2016/04/want-build-empire-like-googles-os/">Source </a>