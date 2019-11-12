---
title : "Placeholder for drafts posts in my blog"
description : "Description of the post"
slug : "draft-post"
draft : true
tags : ["code"]
date : "1995-08-08"
hidden: true
---

## This is a draft post.

Nor again is there anyone who loves or pursues or desires to obtain pain of itself, because it is pain, but because occasionally circumstances occur in which toil and pain can procure him some great pleasure. 

To take a trivial example, which of us ever undertakes laborious physical exercise, except to obtain some advantage from it? But who has any right to find fault with a man who chooses to enjoy a pleasure that has no annoying consequences, or one who avoids a pain that produces no resultant pleasure? 

Nor again is there anyone who loves or pursues or desires to obtain pain of itself, because it is pain, but because occasionally circumstances occur in which toil and pain can procure him some great pleasure. 

To take a trivial example, which of us ever undertakes laborious physical exercise, except to obtain some advantage from it? But who has any right to find fault with a man who chooses to enjoy a pleasure that has no annoying consequences, or one who avoids a pain that produces no resultant pleasure?

```ocaml
scilla_version 0 

import ListUtils 

library HelloWorld 
	fun (msg : Message) =>
let nil_msg = Nil {Message} in Cons {Message} msg nil_msg 
let not_owner_code = Int32 1 
let set_hello_code = Int32 2 

contract HelloWorld 
(owner: ByStr20) 
field welcome_msg : String = "" 
transition setHello () 
	is_owner = 
		builtin eq owner _sender; 
	match is_owner with
		| False =>
		e = {_eventname : "setHello()"; code : not_owner_code}; 
		event e 
		| True =>
		welcome_msg := msg; e = {_eventname : "setHello()"; code : set_hello_code}; 
		event e 
	end

end

transition getHello () 
	r <- welcome_msg; e = {_eventname: "getHello()"; msg: r}; 
	event e 
end

transition multipleMsgs () 
	msg1 = {_tag : ""; _recipient : _sender; _amount : Uint128 0}; 
	msg2 = {_tag : ""; _recipient : _sender; _amount : Uint128 0}; 
	msgs1 = one_msg msg1; msgs2 = Cons {Message} msg2 msgs1; 
	send msgs2 
end

transition contrAddr () 
	msg1 = {_eventname : "ContractAddress"; addr : _this_address }; 
	event msg1 
end


```