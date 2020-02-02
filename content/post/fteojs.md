---
title : "Placeholder for drafts posts in my blog"
description : "Description of the post"
slug : "draft-post"
draft : true
tags : ["code"]
date : "1995-08-08"
hidden: true
---

Finally, the end of JavaScript?

Why JS is successful
At about early 2010, a computer scientist forked Googles V8 js engine and made it run on the back-end/server-side and not the front end.

This could mean that, my barley accumulated skills of writing browser based programs could make me instantly capable of building applications that execute on the server. Hence I hopped the wagon.

JS became very complicated very quickly. It started with package manager Bower it was from fat & i liked work from his collaboration with mdo on Twitter Bootstrap & Medium. So I learned Bower (did I? I have never used it).

Anyway during the Bower reign, npm was quickly picking up & finally took over so & became the default package manager, I had to figure out npm. 

& I haven’t even talked about the task runner wars of grunt, gulp, webpack & <insert latest task runner here>.

BTW, what is Babel? what is ES6, ES7, ES8, ES9?

After that came a tidal wave of frameworks, Angular, Vue and more recently React.

Facebook released React Native that allowed developers to compile apps down to native iOS & Android applications, while they where at it..

GitHub forked Components of Google's Chrome to create Electron, a program that would allow js based UI's to run on a desktop as single programed independent of the browser). 

Now, anyone that has only browser programming skills is instantly capable of releasing apps on iOS, Android, Server & Desktop.

People (future programmers) then flocked in.

This is how JS became king, not because its a language with great features or its well designed but because, people (including myself) enjoy taking the path of least action.

And this is exactly the route of all problems people have with the modern web.

Web obesity
Dependency hell
JS fatigue amongst others


How JS should have evolved.

The JS community has 2 big problems;

1. The lack of respect for standards in the community.

One example is when I look at an html file & its filled exclusively with <div> tags. So much for the semantic web.

It’s like every project uses a different dependency for doing exactly the same things. If am reading through python code, I can at least be guaranteed to some degree that someone maybe using requests

What package manager should I use, yarn or npm? A person doing work in golang will use go get, python projects will most likely use  pip 

2. JS stake holders failing to add new features in the language that seemed necessary as the modern web begun to pick up.

Why do I still need to install a dependency so I can effectively do data binding & routing? Patterns such as these are so frequently used that they should have been simplified the added to the core of the JS syntax.

But now we are helplessly in need of frameworks to simplify these tasks to the level we feel comfortable. Imagine Mithrill's API being a valid vanilla JS.

What philosophy does JS subscribe to? What niche problems does it solve? Is it now a systems programming language?

These questions cannot be answered because the original purpose of JS, adding logic for browser based applications, was given a back seat by its custodians in an effort (unsuccessful one) to make it a systems programming language.

Think about it, a few year back before “JS fatigue” everyone thought the standard way of building websites would be web-components, & it looked really promising but it’s.

How JS becomes legacy.

Some of you think JS will still be on the the top programming languages of choice because the langue is the only one that is widely available in browsers.

People spend a significant amount of time in browsers running  the JS code in them.

I never said JS will vanished in to a pile of "no-longer existent tech". I believe JS will evolve in to more of a runtime & less of a programming language

I think people in need of high-performance code like game engines will turn to C, Rust, Nim and compile code to run in the browser via JS as a target via WASM.

Dart/Flutter actually handles both the need for modern developers have for cross platform hugely & custom UIs.

Dart/Flutter is not just “another framework” it’s more of a graphics engine (think the Canvas API in browsers but for any platform).  It’s a complete piece of tech that has;

A goal (high performance, highly custom UIs)
A philosophy (they like to brand themselves as real OOP)
Standards (well documented suite of declarative widgets more fun to write than HTML)
Standard package manager (pub)

By the way, this article isn’t a sales pitch for dart/flutter. Over the years, UI development (front-end) has become less & less fun for some & I was discovering that I wasn’t the only one feeling this.

Where you one of these people? Try Flutter/Dart. It re-sparked my interest in building UIs aka frontend. That’s why I wrote this for you :)



