+++
title = "On EIP 186 and Ethereum's Greatest Weakness"
description = ""
slug = "on-EIP-186-and-ethereums-greatest-weakness"
draft = "true"
tags = [
    "fintech"
]
date = "2018-03-14"
+++

### The arguments of BTC maximalists are starting to make sense
I have followed the likes of [Beatyon]() & [Saife Dean Ammounis]() (author of [The Bitcoin Standard]()) for some time now & one of the things that facinate ma about their content is that how they consider Bitcoin the only cryptocurrency worth using & lable al other projects (alt coins) like Ethereum as scams.

Reading content from these guys made me initiatly think that they neither understand the value proposition of altcoins nor limitations  bitcoin.


### Halal Pork
[EIP(Ethereum Improvement Proposal) #867](https://github.com/ethereum/EIPs/pull/867#issuecomment-364178634) is titled "Standardized Ethereum Recovery Proposals (ERPs)" from the first comment this proposal will; 

>"Provide a standardized format for Ethereum Recovery Proposals (ERPs), which relate to recovery of certain classes of lost funds"

So what are the examples of the "classes of lost funds" ? from [The Markdown file belonging to the EIP](https://github.com/ethereum/EIPs/pull/867/files/ff62912051fd23d023bb338ba46ab09698d83a20?diff=split#diff-796ab9c4af846b312e8e75cadb5c7bee);

>**Good example** (concise, includes supporting evidence, no negative impact): 
*A crowdsale run by XYZ incorrectly published the testnet address of their crowdsale contract to their public website at the start of the their crowdsale on Jan 19, 2018.  501 ETH was sent by 328 users on the mainnet to the incorrect address between block 4,235,987 and 4,236,050.  See here for the testnet contract, and see here for the transactions to the same address on the mainnet.  See here for a statement made by XYZ on their website.  Because there is a contract at this address on the testnet, it is considered effectively impossible that anyone coincidentally holds the private key. We have verified that all transactions came from addresses with no associated code, so there should be no issue returning eth to the senders.*  

>**Bad example** (not enough detail, no supporting evidence): 
*We accidentally put the wrong contract address up on our website.  Can you please refund any eth sent to 0x1234 back to the senders.  Thanks.*

>**Very Bad example** (not objective, one person’s word against another):
*I sent tokens to X for services and he did a lousy job.  I want my money back but he won’t refund me.  Please help!!*



### Bus Number 
### The greatest Vulnerability ?

