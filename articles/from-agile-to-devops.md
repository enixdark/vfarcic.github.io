# From Agile To DevOps: The History Of Faked Results

Long long time ago, in a galaxy far far away, we would divide SDLC (software development life-cycle) into stages. We would define, plan, code, build, integrate, test, release, deploy, and operate. For the sake of simplicity, I'm ignoring the fact that testing comes after almost every stage and placed it after the integration phase. Business analysts would define what should be done, managers would plan it, developers would code it, and so on. That was the way waterfall worked. If you don't know what waterfall is, you are probably very young and very lucky.

TODO: Diagram

While those stages still exists we managed to shorten them to days, or even hours, instead months or weeks. Agile did that or, at least, that what it was supposed to do. We were supposed to put everyone to the same team, iterate quickly, and deploy often. Did we manage to do that? Some did, most didn't. I can the expression of disbelief on your face. Surely I am wrong. Everyone is agile! Let me present some numbers before you disard my claim of poor agile adoption.

According to studies from 2016, 33% of companies are having agile upstream teams. I'm not going to name the company behind the study. I'll just tell you that it starts with *Fore* and ends with *ster* and let you discover who it is. What is *agile upstream* you might ask? Well... It's a clever way to put a name onto a failure. Now you probably think I'm delusional. Nobody calls anything agile related a failure. Stay with me.

Agile upstream is a collective name for the first half of the SDLC tasks. It includes defining, planning, coding, and building. Integration, testing, releasing, deploying, and operating considered downstream.

The same study states that only 13% of the companies are practicing agile downstream. Do not take those numbers for granted. It does not really matter whether it is really 13%. What does matter is the relation between those numbers. Less than half of the companies employing agile upstream is practicing it downstream as well. Those numbers do not make sense. They are, in a way, a proof that many companies are not being honest.

TODO: Diagram

The whole division into upstream and downstream was invented as a politically correct way to say agile and not-agile. It is a very nice way to distinguish progressive teams from those who are less willing to change. It is a way to admit that agile failed to include half of the departments. Or, maybe, that they failed to adapt. I think that one of the main reasons is coding. The increase in the speed of the upstream teams cannot be followed by those working downstream without coding. The party requires an invitation and only coders got it. If you do not code, you cannot follow the speed. Manual testing is the thing of the past (excluding exploratory), operations based on SSHing into a machine and copying and pasting commands from a Word document is bordering insanity, and monitoring based on an army of operators watching dashboards is a very poor substitute for alerting.

As a result, we got agile upstream teams iterating weekly, daily, or even hourly while those downstream still need weeks to months for a single iteration. The problem is that the total speed is the speed of the slowest. It does not help (much) if half of you are running very fast, hitting a wall, waking up from unconsciousness, and repeating the process over and over again. As long as that wall is there, increase of your speed does not increase the speed of delivery (at least not considerably). Time-to-market is still measured in months.

Such a gap between those involved with upstream and downstream tasks produces friction, and friction produces heat. It is no wonder that "blaming" continues being part of the culture. After all, those teams have very opposing objectives. Upstream teams want to release a feature as soon as it's finished. If possible, they would benefit greatly if it is in production the moment they commit it to a repository. After all, they are in charge of developing those features and want to see business benefits as soon as possible. Downstream, on the other hand, is mostly conecrned with stability. If taken to an extreme, the best way to have a stable system is to never deploy anything. Every change is a potential risk. Long story short, one group would like to deploy all the time while the other would benefit from never deploying.

The result of such a missmatch between those upstream and downstream can take different directions. One possible outcome is the increase in the gap and the increase of the high of the walls that divide those silos. I hope everyone understands by now that such a direction would be disastrous. Even die-hard traditionalists are not proposing decrease in cooperation. At best, they might hope for an extension of status quo.

TODO: Downstream people moving to upstream teams or upstream teams taking over downstream jobs.