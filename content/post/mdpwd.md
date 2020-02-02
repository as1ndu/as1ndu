---
title : "Placeholder for drafts posts in my blog"
description : "Description of the post"
slug : "draft-post"
draft : true
tags : ["code"]
date : "1995-08-08"
hidden: true
---

Quantifying trust-minimization with Hess’s trust theory.

Quantification of properties allows us to measure  how well a system might perform. 

Quantification also allows us to effectively optimize systems, because if we can quantify something, we can know if things are getting better or worse.

In 2017 Balaji S. Srinivasan, described how it’s possible to quantify decentralization of a project based on mining, client usage, Dev commits, exchange volume, liveliness of nodes & ownership of capital by crypto address. 

Decentralization is not however the goal of a particular blockchain project, I think the decentralization metric is great to have an over view of to know how power is distributed within a blockchain project.

Blockchain projects use decentralization (transfer of authority from a single institution to multiple local authorities) to achieve trust-minimization. 

“Decentralization is  what allows Bitcoin to substitute an army of computers for an army of accountants, investigators,  and lawyer’s” - Nick Szabo

Bitcoin is basically designed around  payments. So decentralization of the bitcoin network guarantees that the payment mechanism will be trust-minimized at the same security level.

One thing with smart contract platforms like Ethereum is that, they are plain platforms without a specific application. 

For this reason, the security mechanisms of the platform like Ethereum are detached from the security mechanisms of the applications or “dapps” layer.
This is why the Ethereum network can be decentralized & trust-minimized but the dapps on it may not be trust-minimized.

What is trust-minimization?

Trust minimization is basically the ability for one to mitigate a specific class of harmful agents (also known as byzantine agents)

Liars
Liars are agents that feed the system with false information.

Thieves
These take assets from people  that don’t belong to them without the original owners consent.

Cheats
Cheats (also called defectors) are people that break rules of a game.

Most people mistakenly regard trust-minimization as a binary circumstance where a dapp in either centralized(you are relying on the kindness of  strangers to not rip you off) or  trust-minimized (complete protection from Byzantine agents via cryptography, game-theory or both).  

But trust-minimization is a spectrum & we need ways of measuring it. This is what Zack Hess (author of Amoveo) is trying to develop with trust theory.

It goes as follows;

First we pick a dapp whose trust-minimization we want to quantify. It can be Augur, MakerDAO or EtherDelter.

Then, we outline the mechanisms that make it up.

Each mechanisms is given a scale, the smaller the number the better;

Level 1
These are provably secure cryptographic  protocols often relying on entropy as a security mechanism. Like hashing algorithms & public key cryptography.

In level 1, it doesn't matter how much resources an attacker has as it is practically impossible to guess the source of randomness since the numbers are astronomically large.

Level 1 mechanisms can be considered fully trust-less.


Level 2 
Mechanisms where the costs of breaking a system are are more than the payoff an attacker gets from behaving maliciously. 

Basically these are mechanisms where it's  possible to cheat, but it will be unprofitable to do so.

One thing worth noting is that here, we should have attribution. i.e As on top of it being unprofitable to cheat, lie or steal. We can know who behaved maliciously & can act accordingly (e.g forking, slashing, reduce reputation)

Level 3
In level 3 it is possible to cheat, & the pay off from behaving maliciously is either profitable or net.

Here we can also know who did what & can punish them accordingly like in level 2

Level 4
This is the worst security level (completely centralized). Here it is possible to cheat, profitable to cheat & no one can know who did what for a significant period.

Sublevels
If we have a crypto economic primitive like hash-locks. 
Hashlocks rely on  two things;

a) Blocktime (block headers)

Since blocktime is not based on cryptography but game theory (i.e can be attacked via 51% attack) but it would probably be unprofitable for the attacker, so we put this at level 2.

b) Hashlocks (cryptography)

Hashlocks only release information when a unique piece of data/secret is submitted. If a hash lock is secure, that is using a secure random number & collusion resistant hashing 
algorithm,  we can say it’s protected by entropy & hence put it in the level 1

So now we have a crypto-economic primitive with two level of security. To have a metric that represents both levels of security so we can be aware of the capabilities of this crypto economic mechanism.

For example timelocks would be put in level 2.1  2 is due to the game based block headers, "." Indication a sublevels in the crypto-economic primitive & 1 to indicate it's also has a component of being purely cryptographic. That why we have may rate hashtime locks as level 2.1 security.

Now imagine we have an entire dapp like MakerDAO.

For simplicity reasons, I will say that Maker is basically made up of two mechanisms;

The first component that makes up Maker is the price feed  from a limited oracle source. These oracles have no incentive to keep on telling the truth & we have no way of punishing them incase they mid behave. So we put this on level 4 security.
The second mechanism is a pure smart contracts layer that we can assume is governed by pure cryptography. So we can rate this as level 1 security.

To a it up, MalerDAO from this (over simplified) example we can say that it has a security level of 4.1

When adding different trust levels, it's important that the bigger number comes first, the the smaller number comes second.

Trust theory, clarifies the spectrum of risks that come with  a dapp instead of every one having to read a white-paper, they may not understand. 

Imagine if we had several  dapp rating agencies using Hess’s trust theory. It would definitely improve a lot in terms of insight into the different dapps, what they have to offer in this new world of decentralized applications.






