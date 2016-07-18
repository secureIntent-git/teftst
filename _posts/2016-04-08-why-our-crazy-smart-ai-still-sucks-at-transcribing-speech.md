---
ID: 2575
post_title: >
  Why Our Crazy-Smart AI Still Sucks at
  Transcribing Speech
author: Staff Writer
post_date: 2016-04-08 10:38:12
post_excerpt: ""
layout: post
permalink: >
  https://www.whenitson.com/why-our-crazy-smart-ai-still-sucks-at-transcribing-speech/
published: true
original_cats:
  - >
    ai,voice dictation,computer
    science,machine learning,Gear
original_title:
  - >
    Why Our Crazy-Smart AI Still Sucks at
    Transcribing Speech
original_link:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4eceb3a0/sc/23/l/0L0Swired0N0C20A160C0A40Clong0Eform0Evoice0Etranscription0C/story01.htm
canonical_url:
  - >
    http://feeds.wired.com/c/35185/f/661370/s/4eceb3a0/sc/23/l/0L0Swired0N0C20A160C0A40Clong0Eform0Evoice0Etranscription0C/story01.htm
---
 [ad_1]
<br><div id="start-of-content"><p>In an age when technology companies routinely introduce new forms of everyday magic, one problem that remains seemingly unsolved is that of long-form transcription. Sure, voice dictation for documents has been conquered by Nuance’s Dragon software. Our phones and smart home devices can understand fairly complex commands, thanks to <a href="http://www.wired.com/2016/01/2015-was-the-year-ai-finally-entered-the-everyday-world/">self-teaching recurrent neural nets</a> and other 21st century wonders. However, the task of providing accurate transcriptions of long blocks of actual human conversation remains beyond the abilities of even today’s most advanced software. </p>
<p>When solved on a broad scale, it is a problem that might unlock vast archives of oral histories, make podcasts easier to consume for speed-readers (tl;dl), and be a world-changing boon for journalists everywhere, liberating precious hours of sweet life. It could make YouTube text-searchable. It would be a fantasy come true for researchers. It would usher a dystopia for others, providing a <a href="http://nautil.us/issue/28/2050/what-searchable-speech-will-do-to-you">new form of textual panopticon</a>. (Though with Mattel’s <a href="http://www.newsweek.com/2015/12/25/hello-barbie-your-childs-chattiest-and-riskiest-christmas-present-404897.html">voice-recognition-driven Hello Barbie</a> that listens to the children playing with it, the dystopia might already be here.) Researchers say that functional transcription is only a matter of time, though the amount of time remains a very open question.</p>
<p data-js="fader" class="pullquote carve fader">
	The task of providing accurate transcriptions of long blocks of actual human conversation remains beyond the abilities of even today's most advanced software.	<span class="attribution"/>
</p>

<p>“We used to joke that, depending who you ask, speech recognition is either solved or impossible,” says Gerald Friedland, the director of the Audio and Multimedia lab at the International Computer Science Institute, affiliated with UC Berkeley. “The truth is somewhere in between.” The range of answers about the future of speaker-independent transcription of spontaneous human speech suggests that the joke falls into the category <em>it’s funny ‘cuz it’s true</em>.</p>
<p>“If you have people transcribe conversational speech over the telephone, the error rate is around 4 percent,” says Xuedong Huang, a senior scientist at Microsoft, whose <a href="https://www.projectoxford.ai/">Project Oxford</a> has provided a public API for budding voice recognition entrepreneurs to play with. “If you put all the systems together—IBM and Google and Microsoft and all the best combined—amazingly the error rate will be around 8 percent.” Huang also estimates commercially available systems are probably closer to 12 percent. “This is not as good as humans,” Huang admits, “but it’s the best the speech community can do. It’s about as twice as bad as humans.”</p>
<p>However, Huang is quick to add that this error rate is phenomenal when compared to where the field was just five years ago. And it’s here where he begins to get audibly excited.</p>
<p>XD Huang has been researching the problem of voice recognition for over 30 years, first at Tsinghua University in Beijing in the early ’80s. “We had this dream of having a natural conversation with a computer,” Huang says, recounting a long series of “magic moments” and benchmarks, at <a href="http://www.rr.cs.cmu.edu/">Raj Reddy</a>‘s pioneering lab at Carnegie Mellon, and beginning at Microsoft in 1995. Huang covered the progress, co-authoring a paper with Reddy and Dragon Systems’ Jim Baker in a the January 2014 issue of Communications of ACM titled “<a href="http://cacm.acm.org/magazines/2014/1/170863-a-historical-perspective-of-speech-recognition/abstract">A Historical Perspective on Speech Recognition</a>.” </p>
<p>“Ten years ago, it was probably an <em>80 percent</em> [error] rate!” he says. “To have an error reduction from 80 percent [down to] 10 percent and now we’re approaching 8 percent! If we can keep the trend for the next two or three years, something magic is absolutely going to happen. Predictions are always hard, but based on historical data, tracking records of the community, not one person… in the next two or three years, I think we will be approaching human parity in transcribing speech over a typical mobile phone setting.”</p>
<p>Carl Case, a research scientist on the Machine Learning team at Baidu, works on the Chinese web giant’s own speech recognition system, <a href="http://research.baidu.com/deep-speech-from-baidus-silicon-valley-ai-lab-recognizes-both-english-and-mandarin-with-single-learning-algorithm/">Deep Speech</a>.</p>
<p>“We’ve made some very good progress in Deep Speech with state-of-the-art speech systems in English and Chinese,” Case says. “But I still think there’s work to do to go from ‘works for some people in some contexts’ to actually just works the same way you and I can have this conversation, having never met, over a relatively noisy phone line and have no problem understanding one another.” Case and his associates have been testing their technology in windy cars, with music playing in the background, and under other adverse conditions. Like their colleagues at Microsoft, they have released their API to the public, partly in the name of science, and partly because the more users it has, the better it gets.</p>
<h3>Economy of Words</h3>
<p>For freelancers and other types who want transcriptions and can’t afford the $1 minute rate of traditional transcriptionists, solutions exist. However, none of them are exactly perfect. Programmer (and occasional WIRED contributor) Andy Baio <a href="http://waxy.org/2008/09/audio_transcription_with_mechanical_turk/">wrote a script</a> to slice an audio interview into one-minute chunks, upload the pieces to Amazon’s Mechanical Turk, and outsource the job of transcribing those one-minute chunks to a platoon of humans. It saves money, but there’s a not-insignificant amount of prep and clean-up required. (<a href="https://castingwords.com/">Casting Words</a> seems to have built a business model on the same technique, though it lands right back at the $1 per minute rate.) For an easier to operate crowdsourced interface, there is also the sharing-economy-era site <a href="http://transcribeme.com/">TranscribeMe</a>, transcriptions provided by a small army of manual transcribers, heeding the company’s call to “monetize your downtime.” </p>

A freely available <a href="http://www.fastcompany.com/3050751/elasticity/googles-new-voice-transcription-tool-simplifies-taking-notes">voice transcription tool</a> is likewise built-in to Google Docs for those who would care to experiment. You can play recorded audio on your computer, and the system will do its best to make the proper text appear in a Google Doc. For the five phone interviews conducted for this article, recorded via Skype, only one subject spoke slowly and clearly enough to even register as recognizably transcribed text, with an error rate of roughly 15 percent. Those who only want to transcribe podcasts might have better luck. 
<p>Where currently available transcription technology can’t handle multiple voices or background chaos, reliable software like Nuance’s Dragon <a href="http://www.nuance.com/dragon/index.htm">NaturallySpeaking</a> (also an outgrowth of Reddy’s lab at Carnegie Mellon) has become quite capable at trained single voices. David Byron, editorial director of <em>Speech Technology</em> magazine suggests a technique called “parroting”: listening to a recording in real-time and repeating its text back into the microphone for the software to transcribe. It saves some typing, but is far from instantaneous—and still forces interviewers to relive their most awkward interview moments. </p>
<h3>Speech Impediments</h3>
<p>One person who has doubts about the imminent arrival of long-form transcription technology is Roger Zimmerman, Chief of Research and Development at <a href="http://www.3playmedia.com/">3Play Media</a>, perhaps the only company currently offering a commercial application for automated long-form transcription. Using a combination of APIs provided by vendors Zimmerman said he could not disclose, 3Play’s initial transcriptions average around 80 percent accuracy—sometimes much more, sometimes much less—and are corrected by human transcribers before being sent to customers. “Speech recognition technology is not anywhere near human capability,” Zimmerman says, “and won’t be for many, many years, my guess is decades still.” </p>
<p>“Humans do not speak like text,” says Zimmerman, who has been working with speech technology since the 1980s, when he landed a job at the Voice Processing Corporation, an offshoot of MIT. “I’ve hesitated, I’ve corrected, I’ve gone back and repeated, and to the extent that you have disorganized spontaneous speech, the language model is unsuited for that. It’s the weak component. It’s the component of the system now that’s dependent on fundamental artificial intelligence. What they’ve done with acoustic modeling is signal processing-oriented, and it is well framed, these new deep neural networks, they understand what they’re doing when they decode an acoustic signal, but they don’t really understand what a language model needs to do to mimic human languaging process. They’re using number-crunching to address a much higher artificial intelligence problem which has really not been solved yet.” </p>
<p>But “it’s not <em>thaaat </em>hard,” suggests Jim Glass, a Senior Research Scientist at MIT who leads the Spoken Language Systems Group and who serves as an advisor to 3Play. Glass says, in fact, that the technology is already here. “The way to think of this problem is [to ask] what error rate is tolerable for your needs, so if you’re skimming through the transcript and could jump back to the audio to verify it, you might be willing to tolerate a certain amount of errors. The technology is good enough today to do that. It would take somebody to decide that they want to make that capability available.” </p>
<p>“Part of the problem historically with speech technology is companies figuring out how to make money off of it, and I don’t know if they’ve figured out how to do that yet,” Glass says. He points out that there are toolkits available for developers who would like to play with the nascent technology.</p>
<h3>Enriching Discussion</h3>
<p>The piece that has yet to be combined into commercially available transcription like Google Voice is known as “two party diarization,” a speaker-independent system that can determine who is speaking and what they are saying. One person speaking clearly is one thing, but two people engaging in lively discourse is another entirely. And it is a problem that has been solved, in part, at least in the bounds of scientific research. There is a whole field devoted to it, “rich transcription.” In 2012, the Institute of Electrical and Electronics dedicated a whole issue of their journal, <em>Transactions on Audio, Speech, and Language Processing</em>, to “<a href="http://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=6135542">New Frontiers in Rich Transcription</a>.”</p>
<p data-js="fader" class="pullquote carve fader">
	Part of the problem historically with speech technology is companies figuring out how to make money off of it, and I don't know if they've figured out how to do that yet.	<span class="attribution">Jim Glass, Senior Research Scientist at MIT</span>
</p>

<p>Over a relatively clean phone line, technology could identify the speaker about 98 percent of the time, says Gerald Friedland, who headed the diarization project at the nonprofit ICSI, as the group participated in trials run by the National Institute of Standards and Technology. Running the <a href="http://www1.icsi.berkeley.edu/Speech/mr/mtgrcdr.html">Meeting Recorder Project</a> to test group recording situations, ICSI confirmed that once the microphone is no longer the close-range type provided by phones, the error rate shoots up to anywhere between 15 percent and 100 percent. Friedland points out the range of problems that have to be addressed once one goes past the relatively clean speech of broadcast news into the type of long-form speech that many researchers work with today. </p>
<p>He says, “If you put your cell phone on the table and try to record everything that’s being said and then try to transcribe it, you have a combination of many of these problems: new vocabulary [words], the cocktail party noise problem, regular noise, people overlapping, and people never speak perfectly. It’s got coughs and laughs and there might be yelling and there might be whispering. It becomes very diverse.” Two voice spectrums that often cause chaos in diarization studies fail tests are children and the elderly. </p>
<p>“You can combine these scenarios,” he says. “I think all of this guarantees that a perfect speech recognizer that just listens in like a human will not be achieved in a reasonable time. You and I will probably not see that.”</p>
<p>Which shouldn’t be interpreted to mean that we’re not living in the golden age of speech technology. This month, Friedland helped launch MOVI, a <a href="https://www.kickstarter.com/projects/310865303/movi-a-standalone-speech-recognizer-shield-for-ard/posts/1515592">Kickstarted speech recognizer/voice synthesizer for Arduino</a> that operates without the use of the cloud. “It doesn’t use the Internet,” Friedland says. “You don’t have to use the cloud to do recognition. It can work with a couple hundred sentences and it adapts.” He laughs at Sony, Apple, Google, Microsoft, and other companies that send speech into the cloud for processing. “All of this is exploiting the fact that people think [voice recognition] is so hard that it has to get done in the cloud. If you have one speaker speaking into a computer, we should consider this problem solved.”</p>
<p>For now, Friedland says, most transcription start-ups seem to be mainly licensing Google’s API and going from there. But the field and the market are wide open for innovation at every level, with bizarre kinds of unforeseen societal change coming as soon as a project succeeds. </p>

			<a class="visually-hidden skip-to-text-link focusable bg-white" href="#start-of-content">Go Back to Top. Skip To: Start of Article.</a>

			
</div>
<br>[ad_2]
<br><a href="http://feeds.wired.com/c/35185/f/661370/s/4eceb3a0/sc/23/l/0L0Swired0N0C20A160C0A40Clong0Eform0Evoice0Etranscription0C/story01.htm">Source </a>