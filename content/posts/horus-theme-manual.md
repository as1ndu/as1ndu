---
title : "Horus Theme and its features"
description : "I have used several static site generators, from Jekyll to Lektor and now Hugo. As for now, I really like Hugo but couldn't find a theme that matched my  preferred aesthetics & functional tastes. That's why I made Horus theme."
slug : "horus-theme-manual"
draft : false
tags : ["horus-theme", "hugo", "side-project"]
date : "2020-01-08"
hidden: false
latex: true
---

>"Try to refresh the site before it's finished building.. I double dare you.
Having nearly instant feedback enables you to have your creativity flow without waiting for long builds." - Author of hugo

I have used several static site generators, from Jekyll to Lektor and now Hugo. As for now, I really like Hugo but couldn't find a theme that matched my  preferred aesthetics & functional tastes. That's why I made Horus theme.

This blog posts aims to document the theme's features for those that my be interested in using it.

## Inline Elements

- **Bold Text** is written as `*Bold Text*`
- _Emphasis_ is written as `__Emphasis__`
- ~~Strike Through~~ is written as `~~Strike Through~~`
- `Object.observe()` inline code is written as ```Object.observe()```

## Block Elements

#### Writting a block of code with syntax highlighting
```js
    var foo = function (bar) {
    return bar++;
    };
    console.log(foo(5));
```
```js
    ```js
    var foo = function (bar) {
    return bar++;
    };
    console.log(foo(5));
    ```
```
#### Blockquotes
>"An what makes you prompt for such charity?" - Davie Jones 
```Markdown
>"An what makes you prompt for such charity?" - Davie Jones
```
#### Unordered List
- List Title
    * First item
    * Second item
    * Third item

```Markdown
- List Title
    * First item
    * Second item
    * Third item
```
#### Example of ordered list
* List Title
    1. Fist item
    2. Second item
    3. Third Item

```Markdown
* List Title
    1. First item
    2. Second item
    3. Third item
```

#### Tables 

| Tables        | Are           | Cool  |
|:-------------:|:-------------:|:-----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

```Markdown
| Tables        | Are           | Cool  |
|:-------------:|:-------------:|:-----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |
```

#### Images
![Google](https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_92x30dp.png)
```Markdown
![Google](https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_92x30dp.png)
```

#### Links

Here is a example [checkout](#), you can use footnotes[^1].
```
Here is a example [checkout](#), you can use footnotes[^1].
```


## This is a Simple paragraph

Nor again is there anyone who loves or pursues or desires to obtain pain of itself, because it is pain, but because occasionally circumstances occur in which toil and pain can procure him some great pleasure. Nor again is there anyone who loves or pursues or desires to obtain pain of itself, because it is pain, but because occasionally circumstances occur in which toil and pain can procure him some great pleasure.
***
 
`***` Is used to make a divider


1. _Heading for sub paragraph_

    To have a line break without a paragraph, you will need to use two trailing spaces.
    Note that this line is separate, but within the same paragraph.
    (This is contrary to the typical GFM line break behavior, where trailing spaces are not required.)

    You can also have sub-paragraphs such as this.


**Below are Heading examples.**
# h1 Heading 
## h2 Heading
### h3 Heading
#### h4 Heading
##### h5 Heading
###### h6 Heading

```
# h1 Heading 
## h2 Heading
### h3 Heading
#### h4 Heading
##### h5 Heading
###### h6 Heading
```

## Latex Support

The Horus Theme has the ability to support latex syntax via MathJax, but in order to make it work on a post.
set the `latex` variable to `true` in your font matter. An example is as shown below.

Inline Math $z = x + y$ can e put such as `$z = x + y$`

As for blocks of equations we use `$$ ... $$`

$$
\begin{equation}\label{label}
\frac{\mathrm{d}}{\mathrm{d} x} \int_{a}^{x} f(s)ds = f(x)
\end{equation}
$$

```Latex
$$
\begin{equation}\label{label}
\frac{\mathrm{d}}{\mathrm{d} x} \int_{a}^{x} f(s)ds = f(x)
\end{equation}
$$
```

So the full example of a blog post containing markdown is as below.


```Markdown
---
title : "Math article using Latex."
description : "Demonstration of Latex use in theme"
slug : "math-usage-example"
draft : false
tags : ["math", "calculus"]
date : "2019-08-08"
hidden: false
latex: true
---

Inline Math $z = x + y$ can e put such as `$z = x + y$`. 
As for blocks of equations we use `$$ ... $$`.


$$
\begin{equation}\label{label}
\frac{\mathrm{d}}{\mathrm{d} x} \int_{a}^{x} f(s)ds = f(x)
\end{equation}
$$

```

## Hidden pages & posts

A blog post can be hidden  but setting the `hidden` value to `true` as in the  snippet above. Hidden pages do not get unpublished, they are simply  withdrawn from the posts listing. Search engines are also instructed to not to index the post.

[^1]: The footnote that you want to include goes here.
