I stand by this rather firmly, but first, hear me out before you judge me.

For decades, academics have argued about what makes someone a genius. It's usually called the talent vs. practice debate, and it goes something like this. One side says genius is innate: you're either born with it or you're not. The other side says people can be trained, step by step, until they reach the point we call "genius".

The practice side has some famous stories. Almost a hundred years ago, the psychologist John B. Watson claimed that if you gave him a dozen healthy babies, he could train any one of them to become a doctor, a lawyer, an artist, whatever he picked. (People usually credit this to B. F. Skinner, but it was Watson. And in the very next sentence, he admitted he was "going beyond my facts".) Then there's László Polgár, who decided to raise his three daughters as chess players. Susan and Judit became grandmasters, and Judit became the strongest female player in history. Sofia became an International Master.

Here's the catch, though. Same father, same house, same training, and Judit still went much further than her sisters. So practice clearly mattered. But it wasn't the whole story.

## Before we go further

When I say "genius", I mean it strictly in terms of output: exceptional achievement. Not IQ scores, not how clever someone sounds at dinner. Genius, for me, is what you actually produce.

## Genius as a state

Let's take genius as a state instead of a fixed trait. Think of it as a threshold people cross, rather than a box you're either in or out of. As we go through life, we step in and out of this state. Everyone crosses it, and many times. The people who manage to stay across it for longer end up with the label "genius".

Think of it like a switch that turns on and off. Alongside the switch, there's a stopwatch that keeps track of how long the switch has been on. My theory is that the time on that stopwatch is what mostly separates people.

This also fits with Phillip Ackerman's PPIK theory which, put simply, says that raw mental ability turns into knowledge through the time you spend on something.

But people are born with different starting points too. That's real, and I'm not going to pretend it isn't. Still, someone with a perfectly average starting point can cross the threshold, just like someone gifted can. Whether they actually do depends on two other things: **focus** (how much of yourself you point at one thing) and **friction** (everything that pulls the switch off: distraction, worry, noise, not having the time or the money).

## Testing it (on a computer, for now)

I didn't want this to stay a nice-sounding idea, so I built a model of it and ran 10,000 simulated lives, from age 10 to 80. (I had help from AI tools with the coding.) I used chess as the example, because it's one of the most studied skills there is. Every number I could, I took from published studies: how many hours chess masters needed, how strongly IQ and chess skill are linked, how unevenly achievement is spread across people. Then I checked which versions of the debate could match all of them at once.

Here's what came out.

**1. The stopwatch matters, but on its own it proves nothing.**

![Each dot is one simulated person. More hours with the switch on, more lifetime output.](images/stopwatch.png)

More time switched on means more output, exactly like I predicted. The uncomfortable part: this happens no matter which side of the debate is right. Even if talent decided everything, talented people would still practise more. So "people who practise more achieve more" can't settle anything by itself, and I had to drop it as my main evidence.

**2. Pure practice and pure talent both fail.**

A world where ability doesn't matter at all can't explain why IQ and chess skill are linked (in real studies they are, modestly). A world where talent decides everything makes that link far too strong. What fits is somewhere in between: ability matters, but moderately. Which is pretty close to where I started.

![Grey: everyone. Colour: the top 1% by lifetime output. Left: if talent decided everything. Right: the version that fits the evidence.](images/top1-iq.png)

In the version that fits, most of the top 1% have completely ordinary IQs. Low ability can be a barrier, but high ability gives surprisingly little extra edge.

**3. Luck decides the very top.**

This one surprised me. In most fields, the top 1% of people produce around 10% of all the output. To match how lopsided that is, the model needed luck. So I re-ran the exact same lives 200 times, changing nothing but the luck.

![Each bar is one person's chance of landing in the top 1% across 200 re-runs of the same life.](images/luck.png)

Not a single person made the top 1% in most of the re-runs. For every place at the top, there were about 40 realistic candidates. So the stopwatch gets you into the pool, and luck picks who ends up on top. Which, honestly, makes the word "genius" a bit humbler.

## How are we all equal?

When I say everybody is born equal, I mean it in a philosophical sense. Look at one person on their own and it doesn't make sense; people clearly differ. But humans are social beings. Each of us is part of a bigger group, part of an environment, and the environment hones us. That's really what I mean by friction.

Imagine a kid from a rich household and a kid from a poor one. Look at school alone, and the gap is obvious. But the friction in their lives sits in different places, so they might succeed in different places too.

I tested this as well, and I'll be honest: the strongest version of my idea didn't survive. If rich and poor kids faced the same total friction, just in different places, poorer kids would spend more time on things outside school. Real data say otherwise. Richer kids do more organised sport (it costs money), and in free, unstructured activity there's no real gap either way.

What does fit is a softer version: part of the school gap is friction sitting in a different spot, rather than friction everywhere.

![The gap between the richest and poorest quarter of kids, in percentile points. Lower means more equal.](images/best-area.png)

In that version, the rich–poor gap in school is about 24 percentile points, but in each person's *best* area it shrinks to roughly 5 to 10. So environments don't make us equal. But they decide a lot more of *where* we can be great than we usually admit, especially in things that are free to get into.

## What I haven't figured out

Before I go any further, I want to admit what this doesn't prove.

- It's a simulation. Every number came from someone else's study. None of it is new data yet.
- I can't tell whether talent makes it easier to *switch on* in the first place. The existing evidence fits both answers. Settling it would take a real study with around a thousand people.
- The luck result rests on an assumption: that luck is fresh every year. If the same people turn out to stay on top across their whole careers, I've overstated luck.
- And yes, I'm biased. I want this to be true. I've tried my best to keep that out of my inferences, which is partly why I let the model tell me where I was wrong.

I'm going to keep working on this. If you think I'm wrong, I'd genuinely like to hear why.
