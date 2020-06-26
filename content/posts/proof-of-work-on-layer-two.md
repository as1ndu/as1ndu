---
title : "Proof of work on layer 2"
description : "Description of the post"
slug : "proof-of-work-on-layer-two"
draft : true
tags : ["code"]
date : "1995-08-08"
hidden: false
---

Proof of work on layer 2

Ever since Ethereum launched, they have had proof of stake on their roadmap.

The main decision often cited from this transition is the claim that Bitcoin’s proof of work is a “waste of electricity”.
Even the creator of C++ complained about it.

But now I am talking about why we may need proof of work on layer 2 yet everyone is trying to get rid of it from layer 1. Why?

First, before we think of substitutes to proof of work, we need to acknowledge the role of  proof of work in  a system like bitcoin.

Emin Gun siere (working on avalanche) has a nice micro lecture explaining what proof of work is. 
The conclusion is that proof of work is a Sybil resistance mechanism. Infact it was invented exactly for that back in 1990’s for Usenet.

Basically, it’s roles is to stop one person from spamming the network, rate limiting & making it expensive to generate identities.

So if we are to substitute proof of work then it’s substitute needs to be capable of Sybil resistance or better.

Proof of Stake is capable of  mitigating Sybils on layer one. 
The concerns of Sybil attacks a stretch beyond layer one & layer two.

For instance  let’s say I have a layer 2 based messaging app.  How do you stop infinite streams of messages from spammers?
You have several options 

First you can use the earn.com model where you require every sender to pay  a fee to the recipient. Great but this doesn’t scale properly.

Imagine a Reddit forum where you had to pay $2 every-time you want to post a comment. Even if you can afford it, many people will not & you will be the only one in your forum.

Another option is now to use proof of work. For instance, before you are   allowed to send a message or post on forum, You have also do a small proof of work before you post. 
You can adjust the difficulty of the pow based on the rate at which someone is posting.

This is the technique used by GNUnet an anonymity focused p2p networking service. 

Identity for reputation systems.

Fidelity bonds  have been suggested also as a way to establish reputation in reputation systems. 

They work by someone provably destroying bitcoins, to establish identity. The idea is that destroying bitcoins is expensive, so it’s less likely that the identity is duplicate.

Proof of work can also be as expensive as provably burning bitcoins.
So instead of destroying bitcoins we can just set a pow difficulty & give what ever reputation tokens they deserve to the person that solves this proof of work puzzle.

Do you think proof of work may be useful beyond layer one? Yes or no? Let me know in the comments.







