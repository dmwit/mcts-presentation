# Win any game with these 3 weird tricks. Number three will shock you

In the world of machine learning, there's been a fair chunk of hubbub
recently around the α<sub>0</sub> algorithm. Pioneered by the folks at
Deepmind, it is a triumph in the space of abstract game-playing AIs. One thing
that makes it worth a hubbub is that it doesn't require any expert knowledge of
the game you want it to play; just tell it the rules, and it figures out the
strategy on its own. The algorithm uses Monte Carlo tree search and deep neural
nets at its core. It works pretty well: Deepmind were the first to achieve
superhuman go play, and they have now matched or improved on the state of the
art in a handful of other games, including chess and backgammon.

For some people, machine learning techniques trigger an automatic disdain
reflex. I myself have sometimes said "it's what you use when you don't know
what to use". In this talk, I'd like to challenge that reaction, and convince
you that Monte Carlo tree search is a grounded, principled algorithm; that it's
the obviously correct choice; and that each engineering decision is backed by
solid theory with real LaTeX proofs and everything.

Of course, to do that, I'll have to tell you what problem Monte Carlo tree
search is solving, how it works, and how to turn it into an MLG pro gamer
(batteries and salty trash talk not included). If there's a bit of time left
after the tree search tutorial material, I'll also give a short demonstration
of my home-brew implementation doing a bang-up job of dropping pills and
clearing viruses.

## Will I understand this talk?

You will need some familiarity with basic computer sciencey/mathy concepts to
understand parts of this talk. If you've done any programming before, you
should be fine; if not, you might want to wait until it's on YouTube so you can
fast-forward through any bits you find both unintelligible and uninteresting.
In particular I will not assume expertise in any particular programming
language.

## Will I enjoy this talk?

Many of the people I'm announcing this talk to would be most interested by a
talk about how to make a really great AI for a specific game. I promise you
won't get that: I will only be describing part of the α<sub>0</sub> algorithm
in detail. That part, while fantastic in the property that it requires
absolutely no domain knowledge from its implementor, has by itself pretty
terrible performance compared to more traditional domain-knowledge-based
techniques.

So this talk sits in a sort of awkward spot: it ignores solid, traditional
techniques because I don't like the fact that they need domain knowledge, but
doesn't cover critical bits of the α<sub>0</sub> algorithm that let it perform
well despite not having domain knowledge. If those caveats don't scare you off,
then you'll enjoy the talk immensely.

(...and stay tuned, because I do eventually plan to talk about the full version
of the algorithm! You just gotta walk before you run, you know?)

## How long will I have to suffer?

I expect the talk to last about 30-45 minutes.
