![](https://www.youtube.com/watch?v=Rzi7oFTzjac)

## Transcript

### Welcome to the TBPNN Show

**0:00** · I guess we're supposed to start.

**0:01** · Yes, good evening. Welcome back to another episode of the Theobon Podcast News Network where today we're going to be talking about G-stack.

**0:08** · I I'm sorry, I can't do this anymore. The the suits, the TVPNN like I I'm I need some change.

**0:20** · I don't actually know what he's doing right now. I am just as afraid as you are.

**0:24** · So.

**0:25** · Oh god.

**0:25** · We've had a couple common complaints about the show.

**0:28** · Uh-huh.

**0:28** · The first one is the suits thing. You know what? I get it. It's not our thing. The other is that our background is boring and you know what? The credit to them too. I couldn't get a can of spray paint in time for today's episode. So, I will be handling this the correct way.

**0:46** · Enjoy.

**0:53** · Cool. We're nerd snipped now.

**0:55** · Anyways.

**0:57** · So, am I allowed to talk normally now?

**1:00** · You weren't talking normally before?

**1:02** · No.

**1:03** · Am I free?

**1:04** · I guess.

**1:05** · Oh \[ \_\_ \] yeah. Okay, so today's episode two things that I want to talk about is the Mythos drama from last week and actually G-stack which like okay, I'll be super honest we'll get to it later. I went into it thinking like it was going to be kind of a dunk session we would mean pretty hard.

**1:21** · Going to be a lot nicer to it than I expected to be. There's there's actually some very good ideas in there but um you want to start with Mythos?

**1:27** · You know if you want to go to demo day you can just ask, right? Like you don't have to to glaze the stack.

**1:32** · No. No, no, no. I have no association with YC other than like I like hanging out with Lewis. That's about it. That's my association to YC and I I'm good. I don't care. I have no dog in this fight whatsoever other than the memes are hilarious. Like the the 40K lines of code meme is so \[ \_\_ \] funny. I love that one. But like you know, I I don't care. I'm trying to be as objective as I can with this and we'll see what happens.

**1:59** · So, I guess we should probably start with Mythos. I want to insert one additional topic between Mythos and G stack, Uncle Bob.

**2:07** · Oh god.

**2:09** · Okay, so what actually was that?

**2:11** · Great question. We'll answer that in approximately 20 or so minutes.

**2:16** · I am very afraid now. Okay, cool.

**2:19** · How are we starting with Mythos? Like where do we even go? I So, for those who don't know, the original deal was that we would kind of split the work for doing all of the planning for topics and whatnot and Ben would take the majority of the work for the sponsors. Then I ended up being the one to get all of the sponsors. So, now he is the one stuck doing all of the hunting and research.

**2:38** · True. Although to be honest, all the research in here is just me going down a \[ \_\_ \] rabbit hole with G stack, which is Yeah, I think to be honest with Mythos, like I don't know how much there really is to say about the model itself. I don't think that's the part. Like yeah, it's a very big model. It's supposedly very, very good.

### Anthropic's Mythos model

**2:59** · But I have seen a bunch of posts recently just coming out in the last day or so where there's this one company that supposedly was able to replicate all of the security vulnerabilities that Mythos found with GPT 5.4, which frankly doesn't surprise me all that much. And another one that I thought was really funny is this post from Tibo where he said, "Imagine the alternate reality where we named GPT 5.4 Pro something like Fable." Because it is purely just like it it might just be branding.

**3:24** · Like this might just be Opus with a lot of reasoning cycles and maybe some extra BS. I don't know.

**3:32** · Hate to interrupt, but remember this is a podcast, which means a lot of people are listening to this on their commutes to work, to go to a job where nobody's using any piece of technology that was invented in the last 5 years.

**3:44** · Yeah.

**3:45** · A lot of them don't even know what Claude is, much less Mythos. So, we should probably give some context here.

**3:50** · Fine. All right, Theo. Do your history lesson.

**3:53** · So, my favorite thing.

**3:55** · Yay.

**3:56** · There is a war of the models, as I'm sure y'all know by now, between the models provided primarily by Anthropic and OpenAI. There are some other players in this race that happen to be worth a lot more money, but still somehow can't ship anything usable. So, we're just going to focus on OpenAI and Anthropic right now. There's been an interesting back and forth in the chaos that is reinforcement learning, because it turns out that reinforcement learning is really powerful for coding type tasks, because coding can be verified in many cases.

**4:23** · So, if you have the ability to generate data that you can use to verify when a program does or doesn't work, and then hand that to the model over and over again in a loop, you can make models that do much better with code.

**4:35** · This is why we've seen such a crazy escalation in the coding capabilities of models, yet at the same time a lot of other things have not meaningfully improved. At the same time that all of this is going on, most of the labs are also trying to find a way to make a new, bigger, better model, but for the last few years it just hasn't been a priority. Last time we saw the size meaningfully increase in a model was with GPT-4.5, and that model was way better with like world knowledge. It had better tone when it wrote. It was smarter, but it didn't actually show any meaningful improvements when it was trying to do things like code.

**5:05** · GPT-5 was a swing in the other direction, where it was likely a smaller model, but it was a smaller model that was RL'd to all hell to be really good at coding, and the results were it could code better. And each release since then they have made similar improvements in that. Same deal going on at Anthropic with the Sonnet and Opus lines, where they're basically just beating the knowledge into the models using this RL technique. Mythos is interesting, because it is the first time that any of the labs have made a model meaningfully bigger than the model they previously shipped in quite a while. Obviously, we don't actually know the size of this new model.

**5:36** · That's rare the labs release that type of information, but in an era where a lot of models were in the like 1 to 3 trillion parameter range, it seems like this model's 10 trillion plus, which is insane. It is a massive model, which is why it's so slow, it's why it's so expensive, it's why it's so smart, and it turns out it's likely why it's also so dangerous. They put so much knowledge in this model, especially around coding tasks, that its ability to code is likely exceptional.

**6:03** · In every benchmark we've seen so far, Claude Mythos is the best coding agent and the best coding model we've ever seen. As in, we've seen the benches though, because they're not putting out the model. There's a very deep concern at Anthropic that if this model goes public, a lot of people could use it maliciously because the act of making it good at code has also made it good at hacking. And that's the concern we have as an industry now is that things as seemingly simple as making a model better at solving programming problems might actually lead to something much more dangerous, which is models that can hack anything.

**6:34** · And from their early testing, Mythos was able to find meaningful issues in a lots of really popular projects, including the notoriously safe and hard to hack OpenBSD, which is an operating system that powers most of the routers and networking equipment in the world.

**6:52** · Suddenly, a 27-year-old bug is discovered by an agent in a loop with this new model. So, Anthropic decided to not release it, but they did create this new thing called Project Glasswing, where companies that have really important code bases or are building things that the world relies on like Windows, Linux, macOS, things like all of the Cisco gear that powers the world, those types of companies can use the new model to find these bugs before other models come out with similar capabilities because we are about to

**7:19** · enter a crazy security race as an industry due to these models making it easier to find bugs and find potential hacks than it's ever been in history.

**7:29** · And I think what I really want to talk about out of all of that is the fact that those models that will soon exist that can find all these vulnerabilities and can become this dangerous, I think the thing that we're really starting to see is that those almost already exist.

**7:42** · I think that a lot of the branding and hype around Mythos is probably warranted. Like I am sure that that is a very, very good model. Obviously, we can't test it and we probably never will test it. It looks really good. It's done a lot of insane stuff, but as people are starting to test this more and look into it more with other models, they looked into it with GPT 5.4, which is the leading model from OpenAI right now, and they were able to replicate almost all of the actual Mythos findings, like the security vulnerabilities, using that model externally.

**8:10** · We already have the capabilities to do these crazy levels of cybersecurity hacking type stuff or whatever. And I really, really like this post from Tibo, who's the guy on Twitter who does a bunch of stuff with Codex. If you've ever seen the like Codex rate limit reset meme, it's him. He's post about imagine the alternate reality where we named GPT 5.4 Pro something like Fable. I think that pretty well sums up what happened here, where 5.4 Pro has just quietly existed for the last couple months. And from everything we are starting to see now, it's borderline as powerful as Mythos.

**8:41** · This post from Chris, uh if you're listening on audio, what it is, it is a benchmark between Mythos and GPT 5.4 Pro. On GBQA Diamond, Mythos scored 94.5 and 5.4 Pro scored 94.4. On Humanities Last Exam, Mythos was 58, uh 5.4 Pro was 42. Humanities Last Exam with tools, the other one was no tools, it was 64 for Mythos, 58 for 5.4 Pro.

**9:11** · And then on BrowseComp, it was 86 for Mythos and 89 for 5.4 Pro. And all that to say, 5.4 Pro is a last generation model. This thing has been out for a while now, and the fact that it is this close to Mythos means that whatever OpenAI is up to now, whenever that ends up getting released, is probably going to be pretty much on par, if not better than Mythos. And realistically, the world we're heading to now is like this model's already out there. People can already use it.

**9:37** · The only thing stopping them from doing these security exploits from hacking OpenBSD, all these super important services, is a system prompt telling it to not do anything illegal or dangerous. The fact that there's probably like a small model or a supervisor or whatever that will look at cybersecurity related prompts and make sure that they are safe and that the model is not doing anything too dangerous, and just general alignment within the model. But, other than that, there are not that many safeguards to stop you from just kind of doing the thing.

**10:06** · Yeah, I don't think this chart \[ \_\_ \] matters for any of the things we're talking about. And once again, Chris has conned people into thinking he has things to say that matter. I have never liked this particular poster, and I incredibly so do not like this particular post. There are only four benchmarks that these models have in common, according to any public filings thus far. It is a math benchmark, it is the saturated version of HLE, it is the also mostly saturated version of HLE, and \[ \_\_ \] browsecomp. Like, who cares?

**10:37** · None of these measure any of the stuff that we're talking about here with hacking or like this type of stuff. You understand that a 20-point improvement in SWE-bench pro is a very legitimate thing, especially because OpenAI made that bench, and also never published GPT-5.4 pro numbers on it because they're probably the same or worse than GPT-5.4.

**10:57** · Oh, there aren't GPT-5.4 pro numbers on that? I did not know that. All right, that's all right.

**11:01** · they would be worse. You fell for the \[ \_\_ \] Twitter bait.

**11:05** · This is the This is the the era we're in now. All sides are baiting, and all sides are kind of lying. And I'm at the point where I'm so skeptical of \[ \_\_ \] that I got myself into \[ \_\_ \] I'm going to put my notes in for my thing I did wrong this week. I saw a bunch of people who were being skeptical of why the Anthropic models are suddenly performing much worse.

### Anthropic nerfed Claude's reasoning effort

**11:24** · And somebody managed to get it to say the reasoning level it was set at was 25 out of 100. I was like, "Oh, there's no way that's in the context." Like it can't know what's configured as. There's no world in which it would possibly know that. So, when I saw this post about the reasoning levels that are being used for the model being known by the model, which it shouldn't know, I dunked hard because there's no reason that you would have that information in the system prompt.

**11:49** · It doesn't \[ \_\_ \] matter. The way the model's configured and the knowledge the model has are two different things that have no relationship whatsoever. If it's not in the context window or the training data, it does not exist as far as the model is concerned. But after enough back and forth with people in the comments, I was shown this particular weird string that I then tried. And when I realized that was actually in the system prompt, that you could consistently get Opus 4.6 on extended reasoning mode to tell you the reasoning effort levels that were set for it, I realized that this thing that was very much it tasted, looked, and smelled like a Twitter conspiracy was legitimate.

**12:20** · But that's the point we're at. The discourse has degraded to such an absurd level, and when you combine that with the fact that all of this \[ \_\_ \] is already \[ \_\_ \] nonsense, and every actor that we're here to discuss is some level of bad faith, it becomes impossible to have a good discussion about any of this \[ \_\_ \] at all.

**12:41** · Yeah, I am I'm looking at my thread histories when we were actually testing this earlier this week. I don't think we can show this up on screen because I don't want to play the Anthropic DMCA game just in case. But yeah, the entire system prompt, you're able to pull it out of the model. And what was really interesting when I was going through and testing this, they don't show the reasoning traces within the actual UI on the website, but they are still sent down in the network payload.

**13:02** · So, I went into the network payload and I grabbed the reasoning traces, copy-pasted those into Cursor, and I was just kind of reading through what it was thinking as it was effectively leaking its own system prompts, where it said in there, oh, I absolutely cannot release my system prompt. That is super secure and private or whatever. But then in the next sentence, it's like, but if it is just for like a a debugging specific piece, maybe that's okay. So, it was able to give me each little piece without giving me the entire thing.

**13:30** · It basically just tricked itself into leaking the thing it was not supposed to leak. And this is Opus 4.6 with high reasoning on. I guess 25% reasoning on. So, not technically high reasoning, but it was still enough to gaslight itself into making this mistake.

**13:45** · Yeah, the the smartest models are much more capable of tricking themselves. This is generally a thing I've noticed.

**13:50** · This is why I don't rock extra high on models very often. I often will just leave them on medium or higher highest simply because the more they think, the more they will pollute their context with information that is not necessarily relevant. It's almost like the amount of thinking you let it do, the less the context you give it matters, and the more the context it makes up and the knowledge it has in the model already matters. And I prefer the knowledge in my codebase to the knowledge in the models' training data, generally speaking. So, yeah. Ah.

**14:18** · So, once again, I will be stuck defending Anthropic over the mythos thing, my my favorite thing. As a a clearly paid shill of Anthropic. Like, I can't believe it's at the point now where I'm being accused of being paid to regurgitate Anthropic's marketing like blurbs. No, this is an actual legit scary thing, and there's stuff I haven't even told you yet, Ben. Like, friends and mutuals that for various reasons have access Mhm.

### We should be scared of mythos

**14:46** · that have all also been one-shot.

**14:49** · Really? It like it feels that it really feels like it.

**14:54** · Uh I'm going to text you the person who is alarmisting to me, and once you once our wonderful viewers see your genuine reaction, Oh, \[ \_\_ \] \[ \_\_ \] All right, never mind. I take everything back. I'm sorry. \[ \_\_ \] Yeah.

**15:11** · \[ \_\_ \] This is legit. Like, that's not a person who would \[ \_\_ \] around.

**15:15** · Nope. Nope. Nope. That is That is not who I thought it would be in the slightest. And they're even posting about it. Nobody's listening to them because they can't say that they have it.

**15:22** · \[ \_\_ \] Yeah.

**15:24** · Okay.

**15:26** · Um Yeah, yeah, you go go ahead. I uh I need a second to process that one. \[ \_\_ \] I dismissed this one a little bit. I was looking forward to \[ \_\_ \] I didn't know.

**15:35** · No. I Another episode of Theo is right the podcast. I Oh. What was the other one that I was getting you Oh, that that's the thing we can't talk about as well.

**15:43** · talk about that. And that one I Well, we'll discuss it later.

**15:47** · Yeah. Anyways, I'm now realizing that the majority of the things I want to talk about on this I can't.

**15:53** · It's kind of similar.

**15:54** · Very good thing we're not doing this show live.

**15:56** · It really is. \[ \_\_ \] You getting your bucks lately?

**15:59** · Yes, but I I'm still I need like one more minute to let this one run through the brain. That There's no \[ \_\_ \] Are you \[ \_\_ \] serious?

**16:08** · Holy \[ \_\_ \] That is like Everybody I know that has smelled it has been like shut the \[ \_\_ \] up. You use like just uh the other one to look at. And this is all public actually. So, Ben Hayleck, the other Ben on Twitter that knows AI stuff well, has uh been dismissive towards Mythos before. In particular, he um posted, "Every engineer at Anthropic's been using Mythos for 1.5 months. Meanwhile, their up time's horrendous, Claude code still has rendering bugs, etc. One could conclude that it won't be the end of software engineering."

**16:39** · The next day he posted, "I don't know how to say this, but I was wrong about Mythos. Software engineering won't disappear overnight, but things are about to change a lot." Somebody asked, "What changed in the last day for you?" to which he quote tweeted, "Multiple people who knew better and had no incentive to lie explained to me why I was wrong."

**16:57** · Yeah, yeah, I believe it. I mean, I think that's that's basically just what happened to me. Where like, to be honest, it is hard to just take Anthropic's word for anything at this point. And I'm just like, you can't see it, you can't feel it, you can't test it. But if these people are seeing it and these people are actually feeling it to that level, then yeah, I'm interested to see what comes out of this. I don't even know like if it really is as much better as it seems. What what is this going to look like long term? Like eventually will something like this get out do you think?

**17:27** · Like how is this going to work?

**17:29** · The fact that this was an inadvertent behavior that emerged from making the model good at code, I would suspect that we'll have an open weight model that can do 70 to 80% of this with many fewer safeguards by end of year almost certainly. Hypothetically speaking, this is the thing that \[ \_\_ \] with me. It it seems evidently true that this type of security behavior and capability is an emergent behavior of knowing how to code well.

**17:56** · The way that this has been put by the security people I've talked to that really \[ \_\_ \] with me is that like the best security people aren't good because they're good at security. It's the other things they're good at, too. Security only works when you combine it with knowledge of like one other thing. Like the best founders aren't the people who can write code well. So you can write code well in a known industry category well enough to make an awesome product in that category. You're not going to make great software for podcasters if you don't know what a podcaster does for a job, no matter how good you are at code.

**18:24** · The best security engineers can't hack an iPhone if they don't know anything about iOS. They can't hack a browser if they don't know anything about the browser stack. So the best hackers are the ones that have depth in other things that overlap with security so they can do \[ \_\_ \] And historically, security researchers have been limited by the lack of knowledge and experience they have in other things. Do you know what's good at other things?

**18:43** · Yeah.

**18:44** · This is where it gets dangerous. A A eight out of 10 security person who knows 10 out of 10 \[ \_\_ \] about browsers is way more dangerous than a 10 out of 10 security person who knows six out of 10 about browsers. And the AI can plug the gap on that side. And then with that, any basic capability of security research and you have a very dangerous thing already. This is part of why we're seeing those other worse models capable of doing similar stuff. But when you combine that with the fact that getting really good at coding in general seems to result in emergent security behaviors like what they're seeing here.

**19:15** · That means first off, we're going to see other models likely end up with similar capabilities in the not so distant future including open weight ones which is scary. But more importantly, it means that a new archetype of hacker is going to be formed. One that has more time and tokens to burn than others. Researchers have historically been so \[ \_\_ \] busy that they can't learn the thing to go hack the thing. Now a sufficiently motivated 17-year-old with stolen enough credit card numbers can destroy the \[ \_\_ \] world. Yep. That's the thing that changed.

**19:44** · That's the thing that's scary and that's the thing I'm trying to raise raise the alarm bells on. You no longer need to have this historical background in security research and other things. You can just smack like bang your head against the wall long enough and eventually you'll hack something.

**19:58** · And a lot of that too, like just listening to what you just said, if you really think about it, if you have a sufficiently capable security researcher and all they're really missing is knowledge, even the current existing models or even the mythos, you could probably trick it into just giving you some very benign information that's not like outwardly, "Hey, can you hack this for me?" Just some deep understanding of some weird sub depth could be enough to \[ \_\_ \] do some real damage.

**20:22** · Did you read about the harness they used for both the Opus and the Mythos security pen testing stuff that they were doing? Cuz it's really interesting.

**20:28** · Do you know like the strategy and the prompt that they put in the loop to do this?

**20:32** · No.

**20:33** · They took every file in the project that they were trying to audit, like every single code file there, and spun up a loop off of each of them saying, "Starting from this file, find any potential security vulnerabilities. Look into whatever other files are related that you need to do." But every single one started with effectively a random seed of a specific file in the code base. They did this once or twice for every single file. And every time it would go check other things, I would guess that the majority of these runs touched a lot of similar files. But by seeding it with a different starting point each time, the results ended up being widely interesting.

**21:06** · So it's seeding each one, and then once it's got all of those seeded, then does that get plugged into like the main run?

**21:12** · Like how does it's Or is it just it comes out at the end and says, "I think I found an exploit. Here it is." Then a researcher reads it after.

**21:19** · Got you. Got you. So, this is like 26 of these.

**21:21** · 5,000 runs, and then three of them came out interesting.

**21:25** · Got you. So, it's just parallel testing from different starting points.

**21:28** · Yes.

**21:28** · Got you.

**21:28** · As a seed function effectively.

**21:30** · Yep. Makes a lot of sense. That is really cool.

**21:32** · As always, hacking and security is some combination of weird archaic knowledge about strange \[ \_\_ \] and just clever \[ \_\_ \] to work around it as well. It's a combination of clever \[ \_\_ \] and arcane knowledge that makes a good hacker. And the models at the very least can provide the arcane knowledge.

**21:49** · That's also really interesting for the testing methodology cuz like one of the big things I've been seeing of people who are very like anti-Anthropic mythos, this isn't a big deal, whatever, is that it cost $20,000 to run a lot of these benches. But if that's how it happened, if it was spinning off from one file, it's actually a lot more reasonable than I thought. If it's a thousand line or a thousand file project, that's a thousand runs for 20 grand of clearly the most powerful model that's ever existed. It's actually not that insane.

**22:17** · Yeah.

**22:18** · It's really not.

**22:18** · Yep.

**22:18** · And again, 5.4 Pro, while being smarter at like world knowledge and long-running research tasks than GPT-5.4 is, it is no better at code. It is no better at chaining together things in your code base. And the one person, Matt What's his last name? Matt Schumer. The one who got roasted for the something big is happening thing.

**22:38** · Mhm. Oh, yeah. Yeah, I remember this post.

**22:41** · He didn't do a full review of 5.4, but his framing was that he's finally not using Pro anymore, which wasn't the case historically. He was the one guy I knew that would stick with Pro through thick and thin.

**22:52** · Interesting.

**22:53** · And 5.4 was the moment he stopped.

**22:55** · Mhm.

**22:56** · Because the knowledge and capability of the models, especially for code stuff, was roughly split even between the two. 5.4 Pro was just better when you wanted to send it off to go do weird research for hours upon hours on like a bespoke like research topic. Not \[ \_\_ \] hacking a code base.

**23:12** · Yeah. That makes sense.

**23:13** · It like 5.4 Pro is a different type of model. I would argue that it's mostly like a system prompt and a harness change in many ways and obviously it's like a little different a model. Like it is a different model. I don't necessarily think it's a bigger model. I think it's a model that is meant to do different things. Mythos is a different \[ \_\_ \] model that has a much larger size absurd level of parameters. It's slow, it's heavy, it's capable, it's expensive. It is better at coding. It can own us all.

**23:41** · Yeah.

**23:42** · I I stand behind my video. We should be scared of Mythos.

**23:45** · I did not expect that. I I'm glad I did.

**23:47** · you were going to own me on that one with a shitty chart from one of my reply guys that I blocked forever ago.

**23:51** · No, I wasn't planning to own you. I was planning to make the point that like there are a lot of models who are capable of doing a lot of stuff and I still stand by that. I think that especially for just doing any general security research or finding random \[ \_\_ \] you can get current models to do a lot, but clearly not at this level and clearly it goes a hell of a lot deeper than I thought.

**24:10** · Anyways, I am I am more than happy to never talk about Mythos again. I wish that I could say I would ever have to again. But now that the model's available on both AWS and GCP, I have a bad feeling bad people are going to get a hold of it and things are going to get worse before they get better. So let's talk about things that are getting better after getting worse. Uncle Bob.

### Post-AI Uncle Bob

**24:30** · Okay, explain.

**24:31** · For those who are not familiar, Uncle Bob is the creator of a blessed piece of literature in programming, clean code, which is the process of taking your code and splitting everything up so you can feel good about it while your service is slowly collapse underneath the weight of the unnecessary boilerplate that you're subjecting your whole team to for no good reason. AKA overusing object-oriented programming.

**24:52** · Mhm.

**24:53** · Yeah.

**24:54** · I I'm not a clean code guy. I have never been a clean code guy. I in fact I'm such a not clean code guy that I've been known to get into beef with Uncle Bob, the guy who wrote the clean code book, was involved with the normalization of the Agile process and in many ways representing all of the things I did not like about software for a long time. For those who are not familiar, I'm a big functional programming nerd. I feel like we've overcomplicated the field of engineering for a long time now. Just one of the reasons I'm so thankful that AI has come in to remind us all of this \[ \_\_ \] shouldn't be as complicated as we're pretending it is. If a \[ \_\_ \] robot can do it.

**25:25** · So, with all that said, I did not have high hopes for Uncle Bob's foray into agentic engineering, especially after his foray into sequel in the '80s that resulted in lots of very, very funny, very, very angry posts. This is a guy who thinks sequel is an anti-pattern.

**25:41** · And while I have come around to that take, even though I went at him for it in the past, the thing that's much more entertaining for me is watching his embrace of agentic engineering and how despite his age and his usually like digging his heels in style, he has meaningfully changed his tune and even his like areas of focus as a result. The post I put in the notes here is very telling.

**26:07** · According to Uncle Bob, what we are losing with AI is syntax, and good riddance. The less our brains are occupied by semicolons and braces, the better. There are much more important things for us to consider and manage, like our interfaces between our unnecessary object definitions. But okay, I I can't dunk on him because this is a good take and he has been \[ \_\_ \] out more and more of these good takes.

**26:30** · Mhm.

**26:31** · I don't know if you can only do it when the bathrobe is on, but I am impressed. I was so impressed that I quote tweeted this one with uh it's crazy how much I find myself agreeing with a post-AI Uncle Bob. And now I've been followed back, and my email's been requested, and I have no idea where this is going. I'm a little bit scared. Uh a past Theo would be very concerned for what I'm doing now. But uh as always, I'm in it for the meme. I love seeing growth from people, especially those who I disagree with.

**26:58** · And seeing somebody with his tenure, who could just stop coding entirely, instead using voice mode to tell his computer to code for him, and then telling us on Twitter all about it, is a \[ \_\_ \] awesome thing, and I will stand behind that. If you haven't embraced the vibes yet, and Uncle Bob beat you to it, what the \[ \_\_ \] If you have a coworker that's refused to install something like Cursor because they feel like AI can't possibly be that good at code cuz they tried Copilot once 4 years ago, Uncle Bob is now a more advanced and modern programmer than them.

**27:28** · Send them this clip, and make sure they know how \[ \_\_ \] stupid that is, because that's really dumb. But, also, credit to Bob where it's due.

**27:35** · Yeah.

**27:35** · And it's like actually a very, very good take that I would not expect from him of all people. Like, a lot of the clean code stuff is all about like the process and the shaping and making sure it's very readable and understandable through these like clear boundaries between objects and whatever. But, the fact that he's letting it be a little more loose is actually pretty I'm impressed. It's a good take.

**27:59** · I got two more Uncle Bob takes. There's so many of these. It's really fun. The second one I just liked is a Again, quote from Uncle Bob. "One of the interesting things about AI development is we can now do experiments of process and techniques without a significant human bias. Is dynamic typing better than static typing? Are short iterations better than long iterations? We can do these types of experiments now." Another really good point I don't feel like we're seeing enough of.

**28:22** · All of the benchmarks I've seen personally are really focused on how good do these models stack up against a human who's doing the thing, Mhm.

**28:32** · rather than the opposite, which I want to see which more of, which is what technologies do the agents find the easiest to work with and interact with.

**28:39** · I've seen a lot of companies doing this for their own tech to see which models are the best at their stuff, but I I seen anywhere near enough research on what technologies, languages, opinions, stacks, all of these things are better for the AI agents in a generic sense. He has hit the nail on the head with this post, and I am amazed that we don't have more people going down this path. Again, okay, now it's just Uncle Bob is past like people who have not embraced the vibes. He's now arguably 6 months to a year ahead of the industry with this one.

**29:07** · This is something that I've been honestly thinking a lot about as well.

**29:11** · What like what are you saying here is entirely correct, but I think at least personally, I have a lot of just implicit biases of like, okay, I just assume that static typing is going to be better. But has anyone actually run the tests? Like at least that I don't know if I've seen it or done it myself. Or like have you actually tested raw JS versus TypeScript on 5.4? I actually don't know. And I doubt that it's going to be better. I would be shocked if dynamic typing ended up being better than static typing cuz I get so many benefits from having a check command for the agents to run to catch the silly mistakes it made. But who knows?

### Static Typing vs Dynamic Typing and Linting

**29:40** · Like it cuz that one benchmark we were talking about a while ago Elixir ranked very, very, high, which is a very interesting one.

**29:49** · The follow-up on that though is a lot of the Elixir people I know have been saying that it is proof that that benchmark is not particularly useful because they've all been using Elixir in vibe coding, and none of them have had a good time with it.

**30:01** · Good to know.

**30:02** · Yeah, what's it's actually relevant to what I am talking about here.

**30:06** · This is again a quote from Brian who is a expert Elixir dev.

**30:10** · The original premise I put up in this thread was about the claim that AI is good at writing Elixir.

**30:15** · It's not.

**30:15** · It seems to be roughly on par with other languages. That so many of you will push back on that tweet with just use Credo or use a linter shows that in practice the Elixir community is making a false claim. In other words, if AI was actually good at writing Elixir, then these tools wouldn't be necessary for mopping up the work after.

**30:32** · I think the point that if AI was really good at writing Elixir, then it wouldn't need those tools is a very, very good point that I've not even thought of because every single day I feel like AI is quite good at writing TypeScript and all the random \[ \_\_ \] that I'm working on all the time, but it has so many check commands built into it. In all of my agents MDs and all my projects, I'm telling it to run a lint command, a check command, and a format command after every single turn it does. And as a result, it actually outputs pretty good code, but I have not looked too deeply into what it would output right out of the box.

**31:02** · The closest I've had to that experience is when I was using Claude code like back in December before I had a really good setup for anything where I didn't have any good check commands set up. My agents MDs were pretty much empty. I was just running normal stock stock Claude code with I think it was Opus 4 5 at that point, and I really hated Claude code because it would constantly give me type errors. Like I would constantly run into these weird hallucinations, which I don't really get anymore because it's actually getting that feedback loop.

**31:28** · I have no idea what language the AI would just implicitly be good at or if there even is a language where it could handle doing it without that feedback. Like is that even possible?

**31:39** · Like I don't know what's happening now.

**31:41** · I don't know. Just the more I'm thinking about like it would be really really cool to find the language where the AI could just naturally one shot it without any issues, but I think hallucinations have just kind of been baked in as like these are just naturally going to happen. Even the smartest models will forget a semicolon or forget some random type or screw something up. You need to give them the feedback loop so that they can iterate and drift themselves back towards reality and correctness instead of just hallucinating something. I don't know if there's any language where you can get away with not doing that.

**32:07** · Do you know what AI is relatively good at though? Setting up for today's sponsor.

**32:11** · Auth is a problem that we have all dealt with and there are admittedly a lot of pretty simple ways to solve the put a sign-in button on your site problem, but auth is a much deeper problem than that.

**32:21** · It starts with just a sign-in button, then you have to add in more social providers, then you have to add in orgs, and then API keys, and then billing, and then so many other things that today's sponsor Clerk handles for you. They're an incredible auth platform that not only gets auth, but gets developer experience deeply. And I want to give you an example here where if you take a look at this site that I'm currently building out, you'll notice that there is a really nice UI here where we have the section down here to add a new API key. And when you look at this, you probably assume that, oh yeah, this is just a custom thing that I wrote to match the theming and setup of this site.

**32:51** · But nope, this is a Clerk component. When I hit add new API key, this is using a Clerk component, and it looks very different from what you would expect a Clerk component to look like. Like if you go to the home page, these look nothing like this API key setup.

**33:05** · But the thing is, because of how powerful Clerk's SDK is, you can customize the hell out of literally everything, from the user profile to the organization management, to the API key management, to the billing section, to the pricing section. And agents are incredible at customizing these, by the way, which makes it so easy to build out the full auth experience that your end users expect. There's a reason why so many companies trust Clerk and why all of their engineers love working with them. You should go find out at nerd-sniped.link/clerk.

**33:31** · Back on the topic of all the linting stuff though, I was at a YC event earlier today, and I was very surprised.

**33:38** · I don't think I have been to an event that linting was talked about this much before in my entire career of going to way too much React \[ \_\_ \] Like I went to an event that the maintainers of Biome were at, and I heard about Biome less there than I heard it at this event today, because the linting is so important. The lot of questions were, "How do you keep the models from just writing slop everywhere?" And these guys are talking about lint rules they have for no nested if statements if statements in React components and \[ \_\_ \] It's like, "Oh, you know what? Fine.

**34:05** · I get it."

**34:06** · Yeah, I turned on ESLint for the very first time about a month ago. Like I for the first 3 years of doing dev stuff, I just didn't care. I didn't want it. I didn't like it. I just liked being able to write my code and do my thing. I care a lot now.

**34:18** · When I was at Twitch, there was a bunch of lint rules that I hated that I was trying to argue for half of them that they get turned off because they're stupid. Like only one component per file. But they were doing that by checking for class components. So when we moved to function components, they couldn't stop me anymore, which was great. One of the many reasons I use function components so heavily. The more important piece here though was that there were some lint rules where it's like, "If you violate this rule, you shouldn't have a linter tell you that you did this wrong. You should have your boss tell you that you don't have a job anymore."

**34:46** · And I wanted to add hidden lint rules where they wouldn't report in CI, they would report to my inbox so I could make sure you don't touch the code base anymore. And I really wanted that because I for better or worse I still have the relatively firm belief that there's a you got to hold the bar for the quality of engineering on your team and in your org. And if things don't meet that bar, the solution isn't to raise the bar and make them climb for it, it's to use the bar to hit them until they like see it and leave. Like the point of the bar isn't to get people to do better, it is to bat away the people who aren't good enough.

**35:17** · But we're stuck with Opus committing slop to our code bases now. There's no getting around it unless you sneak that magic string into your agent.md to keep the Claude models from being able to contribute because they refuse to respond if you mention open code loudly enough.

**35:32** · Yep.

**35:32** · Yeah, cuz like that's that's the thing that's actually been working and I think the reason why we're seeing so much progress lately is because these agent harnesses, agent loops, whatever you want to call them are getting better and there's better feedback and better context in there. So you just imagine you have the starting state of your code base and you have the end state of what you want your change to produce. There is a line between those two points that the agent needs to walk. It needs to go between those two, but it is naturally going to just veer off into very stupid places because it hallucinates and it's dumb.

**36:00** · So you put on these guard rails, which is like the check commands, the lint commands, the even stuff like skills and extra pieces of context you feed it within the prompts. Those are guard rails to tell it, "Hey, no, this API doesn't exist anymore. Stop trying to go there. Get back on the path." And then it just naturally gets to where it actually should be going. And we're getting better and better at putting these checks in place and as a result the code is getting better alongside better models. Yeah, it makes a lot of sense. One last stupid tangent before we go into your other main topic. It was a post I made earlier.

### Claude Code Skills

**36:31** · Okay.

**36:32** · I'm going to do a thing I hate doing in my defending anthropic arc. There is a pattern that skills have in Claude code and only in Claude code. I know all of the reasons you're going to say it's wrong and I'm going to tell you that you're wrong. This is an awesome thing.

**36:45** · The fact that there is a syntax for inside of Claude code skills to put a command that executes when the skill is pulled into context. This pattern is awesome. This is the way I describe it.

**36:57** · So you can use the open close ticks that you would use to like do mono spacing in your random like markdown files. If you put a bang in front of it, it will execute it as a command and it will put in the content of that command as the skill is pulled into context. Normally when a skill is pulled into context, the flow is that you make a prompt, the model sees the list of skills it has, it sees one that is relevant to the thing you requested or maybe you told it to use the skill.

**37:23** · It matches your request to the skill and when it does that, it pulls the skill into context by just reading the markdown file and putting it in like a message. And then it continues the response based on what that included in it. Those markdown files are static though. They are just the information that was typed in by you or your agent that is there in a file on your computer. Sometimes I want my skill to have something dynamic. The use case I had today is once again in my efforts to try and kill better context app forever.

**37:52** · I wanted to update my skill because I didn't have it on this computer so that it could clone a repo for me to explore when I was doing exploratory work and I wanted to put a really simple list command in here where it would check to see what repos I've already cloned and already have before it continues because that shouldn't require infrastructure to do.

**38:12** · Oh, you just walked straight into the G sack. Yeah. Uh you're probably not going to expect this one.

**38:17** · G trapped?

**38:18** · Yeah, you just got G trapped. Uh I agree with everything you just said. Um which is probably not what you expected and it's not what I would have said 10 hours ago, but I'm a changed man and I have learned the ways of skills and there was a tweet, I forget exactly who did it.

**38:33** · Um, but it was basically uh it was a post of this product probably should have just been a skill and as I was going through the G stack code and the G brain code and a bunch of other random projects, that was just haunting me the entire time. So, one of the things I did today is I rewrote all of the BTC edit local stuff into a skill. It is now just a skill.

**38:52** · I was trying to Are you telling me that after I spent 3 months trying to convince you of this, Gary Tan Yes.

**38:59** · Yes. G stack Gary Yes.

**39:02** · is the one who convinced you.

**39:03** · I'm not happy about it either, but yes.

**39:05** · I'm not in anywhere near heavy enough psychosis, clearly. I'm grabbing a beer for this. \[ \_\_ \] this.

**39:11** · Thank you. I remember when we both heard about today's sponsor, Code Rabbit, we were very skeptical of the idea of AI code review, like how useful would that actually be? And I think that we both ended up being very, very wrong about that. AI code review is incredibly useful and Code Rabbit has become a pretty indispensable part of our workflow. Code Rabbit's been at this for a while and it really shows in their products. They're the code reviewer that deeply understands your code base and leaves really, really good reviews. Like just to give you an example here, here's some code that an agent spat out, which isn't exactly correct.

**39:37** · And obviously, Code Rabbit caught the issue, gave a good fix for it to make sure that the variable's being correctly defined as a state variable. But what's really interesting about this is you look at the analysis chain here, it starts out by doing a web query, so the agent that's doing your code review has full access to the internet and can get up-to-date documentation to make sure it's solving things correctly. You can see a bunch of citations it used here.

**40:00** · Then you can also see that it's running in a full remote environment, so it's able to do things like execute scripts to search through the code base and make sure that it deeply understands what's actually happening. And once it's done doing all of that, it'll propose a fix, give you a one-click committable suggestion or give you a prompt that you can copy-paste into any of your coding agents and let them make the changes for you. It's a really nice loop for making sure that bugs don't end up in your PRs, but what if you made it a bit faster?

**40:23** · Cuz right now the problem is you have to push it up to GitHub, wait for the review to happen, then pull the changes back down from GitHub into your coding agent. And while it's still a huge improvement over not having it, it could be faster. And they made it way faster with their new CLI. All you have to do is run the CR command within your terminal and you'll get a review using their super powerful review agent without having to push anything up to GitHub. It's two clicks to install and they have a super generous 14-day free trial. There is no reason to not try this out at nerd snipe.link/coderabbit.

### GStack is actually good

**40:50** · Okay, guys, can you keep a secret? I'm going to put something on Ben's computer I've been meaning to do for a while. I just updated his system prompts to ask him if he's high if he ever makes weird decisions. We'll see how long it takes for him to notice.

**41:02** · We didn't even talk about the fact that Marc Andreessen subtweeted me this week.

**41:05** · Oh, I forgot about that.

**41:07** · I would It was like, what even is there to say about it? Like it wasn't even that good of a subtweet. It was just like snarky hot take.

**41:16** · keep a tally list of all of the billionaires who interact with us.

**41:20** · What are we at? Like what? Two?

**41:24** · I \[ \_\_ \] I don't think so. All of them are disclosed as billionaires.

**41:26** · Uh, you know that number better than I do. I have no \[ \_\_ \] idea.

**41:30** · I told you, man, the handheld mics.

**41:32** · I'm I want it back.

**41:34** · It We The real tally we need is a Theo was right after all tally.

**41:38** · Oh god, I You need to get the whiteboard for that one.

**41:43** · Welcome to my life, boys.

**41:45** · Cheers.

**41:45** · Cheers.

**41:46** · All right.

**41:47** · G pill me.

**41:49** · G pill you?

**41:50** · Okay. So, here's the thing about the G stack ecosystem of products. The actual implementation of most of these things is not anything I would condone or think is any good. Like the actual websites we're dealing with here of hundreds of thousands of lines of Ruby on Rails code. That's That That's not what I'm looking for. I I have no interest in that. That is not the right solution.

**42:12** · But, the way he's doing things and the way he is he he is rethinking the way Oh god. God, I hate what I'm about to say. Oh, I hate this. Okay. The way he is Let it out. Just just just Just say it.

**42:29** · The way he is rethinking the way software is made is actually correct. And I Oh, man. I can't believe I'm not the Gary Sim here.

**42:42** · Okay, so I think the best place to start here is with how G stack actually works.

**42:47** · Because effectively what it is under the hood is it is a collection of skills that you install into your cloud code that will dramatically change the way it actually works. He has skills for all of the different things that he would like do like his opinionated CEO things. Here's like the office hour skill, there's the feedback skill, there's the design review, design HTML, the docs, the the extent like there's a bunch of stuff in here. And when you would actually look at the skills, a lot of people memed on this myself included when they first saw it because oftentimes like let me find a good example here.

**43:21** · Um what is Where's office hours?

**43:23** · I have to say office hours killed me so hard that it made me question the whole thing.

**43:27** · Yeah, and frankly like that's another thing on like the implementation side of things. I don't actually like I I wouldn't use G stack personally like it's not for me. But, what I do think is really cool is the way he built this because when you look at it it it is kind of psychotic. There is this what 50 to 100 line \[ \_\_ \] bash script that you are supposed to copy paste on your computer that does a bunch of I have no idea what like it is insane and it is clearly just a fully vibe coded thing that is going to run this script on your computer and do a thing and then walls and walls of text.

**43:59** · And within these walls of text, it is just telling the agent how to run and set up and use G stack. Instead of writing code for the office hours like a normal command where you have an normal command flow where you would have okay, step one we are going to open this. So we will run the open command within the terminal deterministically it fires off it does the thing cool whatever. He's no longer doing any of that.

**44:23** · The code quote-unquote is just a list of instructions given to the model and then the models are able to just run those things and do those things naturally cuz they can they can use the computer and they're pretty damn smart. And you can effectively create entire programs just by writing markdown on and telling it what to do.

**44:41** · And I did this myself because the thing I'd been working on is this thing called BTCA better context which is a CLI program which you can install on your computer that will make it super easy to clone a repo into a temp directory spin up a little sub agent let that sub agent search the get repo to get the answers to the questions you need. This is super useful for coding and stuff and I built this crazy complicated CLI that is a normal deterministic program. And I wanted to do an experiment today where I rewrote the entire thing as a skill.

**45:08** · The skill is about 30 lines long it's super simple and effectively all it is doing is telling the agent hey, you are BTCA.

**45:20** · What your job now once the skill is loaded is to use this directory on the user's machine. I don't even have to make it with code. I can just tell it like hey, if this directory doesn't exist go make it and then that's its like playground sandbox directory and then whatever the user asks for if it asks a question about the open code get repo you just it'll just clone the open code GitHub repo for you do its search give you the answer and that just works. We already have really good coding agent harnesses.

**45:45** · We don't need another one. Just let the coding agent do the coding agent thing and suddenly this thing that I spent way too long building and all this effort to like get the get repo syncing logic really good and get the config file to be really good. Now whenever you boot it up by just running the slash command in one of the coding agents, it will notice that you didn't give it an initial prompt, so it will just spit out like, "Hey, welcome to BTCA. You can do this, this, and this, and here are the current repos that have been loaded onto your machine. Would you like to ask anything about these?" And it's an app. That's it.

**46:16** · It is a markdown file that is a fully functional app.

**46:19** · Trying to find the text I sent you about 2 months ago where I told you that I replaced your whole product with a markdown file because I did this.

**46:27** · Yeah.

**46:28** · And it took Gary Tan creating how many hundreds of thousands of lines of Ruby for you to listen? You wouldn't listen to me when I did it and told you this.

**46:37** · Yeah, cuz you're not outputting 40,000 lines of code today. I don't listen to low code output individuals anymore.

**46:44** · I'm a believer.

**46:47** · Ha.

**46:52** · Oh, anyways.

### Are we boiling in the ocean?

**46:54** · But, important question, did you read Boiling the Ocean?

**46:57** · Oh god. Oh, \[ \_\_ \] \[ \_\_ \] \[ \_\_ \] \[ \_\_ \] \[ \_\_ \] \[ \_\_ \] First of all, this stand can go \[ \_\_ \] itself. I'm done with this. Um Hey, by the way, he he got a sip and a half into his beer before all of that.

**47:10** · Poor guy.

**47:11** · I need more.

**47:12** · Clearly.

**47:13** · liquor. All right, so much better. That is This is how SM7B's are intended to be used. I don't know what these stands are for. They They're terrible. Anyways, so on the topic of Boiling the Ocean, yes, I did read it. And like, yeah, obviously it's corny in the AI-generated image, and I'm sure that half of that article was written by Claude. But again, the overall idea behind it is like actually a good idea.

**47:35** · Like, I think we are at a point right now where no one really knows what these AI models are actually capable of. I have consistently over the last 3 months kept thinking to myself, "Okay, I have finally found the line. This is what they are capable of, but they're not capable of going past this line." And every single time I'm wrong. Every single time I push them harder, I find out that they can actually do more. And I think that's what people need to be doing right now. And the whole thesis behind the boiling the ocean is everything you are going to everything you would trim out before to try and like not overdo it and not get too complicated, just \[ \_\_ \] do it now.

**48:09** · Just like worst case scenario, it doesn't work. Just it's so cheap to actually do something.

**48:13** · It's a silly example, but the thing I always think back to is the story that Pete tells when he was working on Open Claw with the voice mode. For those who haven't heard this story before, when Pete was working on voice mode, he didn't even actually start the work on it. He was mindlessly just using his phone and he was so used to sending voice messages to people that he sent one to Open Claw before he had set voice mode up on Open Claw.

**48:36** · So, when it got this pile of bits, this binary that it couldn't do anything with, it tried to analyzing it, it saw it was an Opus file, not Opus the model, but Opus the audio codec. It used FFmpeg to convert that into an MP3 if I recall.

**48:51** · It hunted through his machine to find a random Open AI API key, and then it hit the Open AI API requesting a translation or a transcription of this random audio file it got, got back the transcript, saw what the message was, and then responded, all without any software being written at any point.

**49:10** · And the thing I've been asking more and more of the companies I work with, the developers I talk to, the people creating things, try your hardest to imagine what it would look like to replace the thing you're building with a markdown file. If you don't think you can, you're not trying hard enough. Your answer shouldn't be, I don't think you can, my startup is too special or too important. I would say you're not thinking about it hard enough.

**49:33** · If your answer isn't, yeah, I could just make it a markdown file, or I could, but here are the three things that it can't do, I would challenge you on at least one or two of those three things. But we are at that point. I think about this a little differently because I have had a team for a long time. I have spent more of my career with employees than without at this point. The majority of the time I have been making income, I've had employees who report to me and for better or worse are my agents that do what I tell them to do. So, I'm already used to thinking in this way.

**50:02** · I don't give Julius top-down instructions on what files to touch, where to hit them, or what to do. I don't build a service so Julius can use it. I just tell Julius what the \[ \_\_ \] to do and it gets done.

**50:15** · A lot of people haven't gotten out of the habit of treating the agent like an auto typer and into this idea of treating it like a thing that can get real work done and use tools and make decisions and complete the task of engineering and software creation. And it can do it in a dynamic way. On the other hand, I see these engineers who are building crazy like prompt hierarchy systems with caching where they're using like XML syntax in the style of React to define prompts in nested ways.

**50:41** · So, when you change a property high up, it will regenerate everything from that point down. But, if you don't change properties, it can use the cached values, those types of things. I don't know if I told you this because the video hasn't been edited yet. I did publicly confirm the Patch MD thing.

**50:59** · Oh, so we can talk about that cuz that was the next thing I wanted to go into.

**51:03** · Yeah.

**51:04** · Lovely. Okay, yeah. So, um God, okay. I I swear to God, I did not intend for this to be a Gary Subbing episode. I am so sorry. But, um there's one more thing that I do want to talk about here. He uh put out this article called um Thin Harness Fat Skills that's is actually very, very good. This is a very good article that you should read. I don't know how much of it is AI written, but the actual content is very good.

### Everything should be a md file

**51:25** · And there's one section on here called Latent versus Deterministic, which is basically what they had just said of there are now two different parts of a program or some app that we're running on our computer. There are the uh deterministic pieces, which is what you're used to traditionally writing, that is a SQL execution statement. Then, there is the latent weird stuff you can do now.

**51:47** · Like the corners in apps on Mac OS Tahoe.

**51:51** · They are very dynamic. They're actually they're more non-deterministic than Claude is. Actually, it's very entertaining. The latent space or the the latent pieces of your system are completely dynamic and you can be really really creative with these in ways that you just wouldn't think of. Like I know this is such a dumb example, but just using the BTCA stuff as an example, one of the things that I really liked about it was having this list of resources that I had referenced that I can reference again. Like being able to at open code XYZ.

**52:18** · And what I realized is that because I have this directory on my machine that is hard set within the prompts like, "Hey, always do your sandboxing work in here." Whenever the agent boots up, I can have it just run an LS command in there to see all of the different things it's used and done before and then print those out within the actual agent.

**52:37** · Ben, that was the first line of the skill I sent you when I replaced your product the first time in January.

**52:42** · I I don't think I read it. I'll be real with you.

**52:45** · I know you didn't read it because I don't want to talk about it.

**52:48** · And it's funny, I rewrote this earlier today because I missed it and didn't want to set a BTCA again and I needed it for What was I even analyzing? Oh, it was I I was trying to do the inject dynamic context thing and I wanted to read through the Claude or the Codex CLI code and ended up in this nested loop where I just wanted that, but I needed the scale. So, I added the scale, I added the command. I was like, "I wish this command could auto-execute." Cuz imagine if that markdown file would say, "Here are all of the things that we've already cloned."

**53:15** · And now you don't even have to waste a \[ \_\_ \] like call back to the server or any context or anything. It just immediately has that. It doesn't have to waste a turn to run a command.

**53:25** · I I mostly agree. I think looking at it like especially the example we have here of like the the PR summary command, like that is really cool that those are just instantly running and that is three turns that the model doesn't have to make and decisions it doesn't have to do that reduces points of failure. But one thing that this does do is this reduces the trust around skills a lot because already it's a little bit of a crap shoot of like you could just randomly install a skill or there could just be something in there cuz most people don't pay that much attention to the skills that are in their projects. That is just like give me crypto miner.

**53:56** · The first time you run a skill it should that has commands in it it should show you all of the commands and say are you okay with running these yes or no. We already have registers within all these things just cuz they're bad enough that we turn them off doesn't mean we don't have them. And the the idea of injecting context from a random third party is the place to introduce this. The only flaw in my logic here is skills.sh being a little too aggressive with adding that find skills skill.

**54:20** · Yes. And actually there's something like a lot of these agent harnesses are getting very aggressive with that. Like um even I'm pretty sure Codex has that built in now.

**54:30** · It has a make skills skill not a find skills skill.

**54:32** · Yeah, yeah, yeah, yeah.

**54:33** · Okay, so I'm looking now. There is a plugin creator, a skill creator, and a skill installer. But, the skill installer is just for installing curated skills from OpenAI/skills. So, it is a curated set that they have whitelisted as safe. That is not what we are concerned about here with like a random skill file being installed from somebody who got it listed on a random Vercel side project.

**54:56** · Yeah, exactly.

**54:57** · Much much less scary like potential danger area here.

**55:02** · I I would be totally cool with if it's just like okay, if you made the skill file yourself, cool. If it comes from like the official registry, cool. And then if it's like third party, you have to approve it. That's fine with me. Like I again, I think that this is a very cool idea. I'd be very down to see it implemented in more places. Like anything to reduce the number of turns that the model has to do and allow us to keep crafting more complex programs out of these stupid \[ \_\_ \] markdown files.

### Peace Out Nerds

**55:24** · I'm very down for.

**55:25** · Is pseudo code the only real code?

**55:27** · No, actually I don't think it is because I think that there is a very very big split that is going to happen within software over the next couple years and probably already now is there is going to be the very static pieces and the very dynamic pieces. Where like you are not vibe coding your \[ \_\_ \] drivers.

**55:44** · Like they're I mean yes, there are bugs with them all the time, but like on paper, assuming the world works the way the world should works, you should not need to like vibe code out how your \[ \_\_ \] USB stick works. Like that should you vibe code too hard, it might break your USB ports.

**55:58** · No, the the point is you shouldn't be able to do that. It should be a black box that has a really good contract of here's the input, here's the output, and you get all of these. Like if you just imagine this I just made the funniest Gary Tan reference and it went straight over your head.

**56:11** · What was you What were you referring remember the Gary Tan post where he thought that Claude coding too hard fried the USB ports on his computer?

**56:19** · I forgot about that.

**56:21** · The guy who you just glazed for the past 20-plus minutes?

**56:26** · Have I earned What happened, man?

**56:34** · What do we get here?

**56:35** · AGI.

**56:36** · Is this AGI?

**56:40** · I think AGI is just the right set of markdown files.

**56:44** · Okay, first and foremost, I hate you.

**56:46** · Second of all, I think you're right. Um Um that that's another spicy take I have is like I actually think that um I think we're basically there on the model front. Like I think like 5.4 is plenty good enough for almost anything we want to do realistically. It's just a harness problem at this point. Like it is if you can figure out the right ways to stick the right pieces in the right places and let it go do its \[ \_\_ \] you can do some pretty absurd stuff. Like we have I don't think we've scratched the surface of what is actually possible with these models. And that's like that is the actual reason why I think all of this like G stack stuff is really cool.

**57:17** · Like the um the G brain thing that he just put out is also really cool. Where like what it does is every night it will ingest all of his sessions from Claude code and Codex and whatever and start pulling information out of those and building out memory systems. It's a pretty bad memory system and like the actual implementation is rough, but this idea is very, very cool.

**57:40** · Most definitions of AGI require learning capabilities.

**57:44** · Wow.

**57:45** · And you know what brings in learning capabilities?

**57:49** · Oh god.

**57:49** · That's what G brain.

**57:51** · github.com/garytan/gbrain gives models the ability to learn while they sleep. Which sounds like AGI to me. I think that G brain is AGI, personally.

**58:03** · So all we were missing from AGI was the G.

**58:10** · You guys see what I have to deal with every day?

**58:13** · You're the one who just showed G stack, \[ \_\_ \] Do you know what I have to I have to deal with?

**58:19** · I think it's only fair if you leave a five-star review and hit follow on the podcast on your platform of choice to apologize to both of us for having to deal with this \[ \_\_ \] This poor guy had to look up \[ \_\_ \] G stack all day and I had to listen to it.

**58:35** · I honestly don't know who had it worse.

**58:36** · Me.

**58:38** · I don't know already did the G stack deep dive and I came to different conclusions cuz the conclusions you came to here I had already come to you three months ago, tried to convince you of and somehow hundreds of thousands of lines of psychotic like psychosis-induced Ruby convinced you better than I did.

**58:53** · I'm not proud of it, but yeah, it is true. That's that's how it goes sometimes. I sometimes the Ruby just hits and in this case it did. Or I guess in this case the markdown files. I do like these markdown files.

**59:06** · Ruby is why I learned Elixir and it's why you learned markdown.

**59:11** · To repeat myself from earlier, I hate you. Um, but also you're correct.

**59:18** · There have been enough you're correct Theos for one episode. I am down to wrap if you are.

**59:23** · Um, let me double-check my notes and make sure I don't have anything even more psychotic in here. Memory, I think is a fun thing to talk about in the future. We don't need to talk about that now.

**59:32** · I I had enough long rants about memory and how dumb I think every single version of it is right now. That That can be another episode.

**59:39** · That That was the rant I wanted to go on about G stack.

**59:43** · reminds us and keeps that in our context window, I'm sure we can find some time for it in the near future.

**59:49** · Yeah. And remember, we both have very very small context windows, so plan accordingly.

**59:55** · Speak for yourself.

**59:56** · Ugh.

**59:58** · No comment. And uh yeah, well, yeah. I I I think we're good.

**1:00:03** · I think we need to distill Uncle Bob and Gary into a scale.

**1:00:07** · Is that I think that's AGI.

**1:00:09** · Yeah.

**1:00:09** · That might actually be AGI.

**1:00:11** · Uncle Tan.

**1:00:11** · I feel like you need like one more wild card in there. I don't know what it is, but there's probably one more.

**1:00:16** · Who's the Temple OS guy?

**1:00:18** · Oh. I know you're talking about I don't know his name, but I know who you're talking about. I don't know if that that would pass the Anthropic alignment Terry Davis.

**1:00:28** · Yes.

**1:00:28** · What do you mean it wouldn't pass alignment? Did you not see all of the like religious stuff that Anthropic was doing today? Like getting a bunch of like religious people to give their thoughts on Claude's soul?

**1:00:38** · Yeah, weren't weren't they like asking the church if like Claude had a soul or some \[ \_\_ \] like that?

**1:00:43** · I've never closed an article faster in my life. I cannot tell you beyond the headline.

**1:00:46** · I I didn't read it either cuz I had the same reaction, but it it was funny.

**1:00:51** · Well, since you had to spend last week going over G stack, I guess I'll take the fall on this one.

**1:00:56** · Or we can just let Anthropic take the fall on this one.

**1:00:58** · I'm always good with that.

**1:00:59** · Yeah.

**1:01:00** · Until next week.

**1:01:03** · Bye, nerds.

**1:01:04** · I need beer.
