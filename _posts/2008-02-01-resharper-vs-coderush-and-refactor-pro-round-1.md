---
layout: post
title: Resharper vs CodeRush and Refactor Pro - Round 1
date: 2008-02-01 18:50
author: John
comments: true
categories: [All]
---
<P>I've developed .NET applications with both of these products in the past and they both have some great features that save a ton of time. It had been a while though since I last did a comparison, so I decided to put them up to the challenge once again. Here are my initial thoughts on the best pros and cons of each. They both have some great refactoring features, however they also each had some good differentiating features too. I've just started my revisit to these 2 products which I plan on comparing in real development over the next few weeks. But here is my initial thoughts on the 2 of them ...</P> <P>Top 3 features that <A href="http://www.jetbrains.com/resharper/">Resharper </A>has over <A href="http://www.devexpress.com/Products/NET/CodeRush/">CodeRush</A>/Refactor Pro:</P> <OL> <LI>Analysis icon (shows code errors before you build) <STRONG>This is just awesome!!!</STRONG> <LI>Find Usages (finds all usages of a class, interface, etc.) <LI>Optimize "usings" (removes unnecessary using statements)</LI></OL> <P>Top&nbsp;4 features that <A href="http://www.devexpress.com/Products/NET/CodeRush/">CodeRush</A>/Refactor Pro over <A href="http://www.jetbrains.com/resharper/">Resharper</A>:</P> <OL> <LI>Better templates out of the box (helps write code faster) <LI>Quick Find (helps find a method, property, class or whatever very quickly) <LI>Better visual enhancements (blocks the regions well, blocks code nicely, auto-highlights easily, shows code flow nicely with visual cues) <LI>Use of markers</LI></OL> <P>If you could combine some of the features you would have a great product! I love <A href="http://www.jetbrains.com/resharper/">Resharper's </A>analysis tools!!! If you ahven;t seen it, try it out. What they do is check your code for compile errors and even for warnings while you type. So before you even build your code you will see an indicator that shows&nbsp;green (all is well), orange (warnings exist), or red (something is amiss). Warnings could be something like you declared a field that you never use, which is helpful for cleaning up your code. </P> <P>The Find Usages feature of <A href="http://www.jetbrains.com/resharper/">Resharper </A>is incredible, too. I recently had to work on a few major refactor jobs where I had to change about a dozen classes and every place that used them. This ended up effecting about 50 files as the application was very OO and the levels of inheritence and interface usage was deep. The Find Usages feature of <A href="http://www.jetbrains.com/resharper/">Resharper </A>made this soooooooo much easier on me. Whenever I&nbsp;changed a class I first looked up all usages of it so I could make sure I tested those paths as well. When I changed the signature for methods or constructors, it updated the usages for me! Very slick indeed.</P> <P>These 2 features of <A href="http://www.jetbrains.com/resharper/">Resharper </A>alone are just incredible, IMO.</P> <P>I do find that the templates in <A href="http://www.devexpress.com/Products/NET/CodeRush/">CodeRush </A>to be much better out of the box. Writing code with them is so much easier than without. For eaxmple, to declare a local variable&nbsp;I just type "fi[space]" and it inserts a int for me. If I type "pi[space]" it inserts the template for a full Property with get and set accessors. Very slick. There are a ton of single and multi key templates that you can use. I plan on testing them all out to see how they compare to <A href="http://www.jetbrains.com/resharper/">Resharper</A>, but so far they seem a ton better in <A href="http://www.devexpress.com/Products/NET/CodeRush/">CodeRush</A>. </P> <P>OK, maybe its trivial, but I have to admit that <A href="http://www.devexpress.com/Products/NET/CodeRush/">CodeRush </A>has some nice visual features that caught my eye right away. It makes regions look more visually disparate than with <A href="http://www.devexpress.com/Products/NET/CodeRush/">CodeRush</A>. It does this by making the region be a highlights rectangle when closed. Does it help me code? Nah, but its a nice visual feature. But I added it in this post because it maakes me wonder why other products don't offer this (or maybe they do and I am not aware). <A href="http://www.devexpress.com/Products/NET/CodeRush/">CodeRush </A>goes further by putting icons next to classes, properties, methods, interfaces, etc to help denote if they are private, public, internal or whatever. Again, another nice feature but it isn't likely to help me code faster. Where it is smarter is when you click on the icon of, say, a public class, it gives you a pull down list of other options besides "public". So you can change a class to "private" in this manner. The best visual feature may be how it shows control of flow, though. For example, if you have a return statement <A href="http://www.devexpress.com/Products/NET/CodeRush/">CodeRush </A>shows a green arrow next to the return. If you click the green arrow a graphic appears that points you to where the return statement exits the routine. Similar graphical features also exist with the continue, break and exception throwing commands. These are very slick.</P> <P>OK, so far I am still on board with <A href="http://www.jetbrains.com/resharper/">Resharper</A>. I think the featureset with <A href="http://www.devexpress.com/Products/NET/CodeRush/">CodeRush </A>is more extensive that Resharper and frankly it look a lot fancier that <A href="http://www.jetbrains.com/resharper/">Resharper</A>. But I just don't think I can live without the Find Usages and Analysis&nbsp;features of <A href="http://www.jetbrains.com/resharper/">Resharper</A>. The template features of <A href="http://www.devexpress.com/Products/NET/CodeRush/">CodeRush </A>are <STRONG>very </STRONG>appealing though. Maybe someone will create a tool that combines the best of both worlds from these products. </P> <P>Stay tuned ... I'll post more about how my experience goes with both of them.</P> <P>For me, Round 1 goes to Resharper on a 2 to 1 decision.</P>
