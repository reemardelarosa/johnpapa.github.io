---
layout: post
title: Incrementing in .NET (i++ vs ++i)
date: 2008-02-01 18:50
author: John
comments: true
categories: [All]
---
<P>I was working with some friends on some unit testing when we recently ran across an issue that was caused by an uninteded use of an incrementor (++). It was&nbsp; quick fix but it is also something I have seen quite often, so I figured I would jot my thoughts down while it was fresh in my mind.</P> <P>So we've all seen the common for loop in .NET, looping a finite number of times.</P> <DIV style="BORDER-RIGHT: windowtext 1pt solid; PADDING-RIGHT: 0pt; BORDER-TOP: windowtext 1pt solid; PADDING-LEFT: 0pt; FONT-SIZE: 8pt; BACKGROUND: white; PADDING-BOTTOM: 0pt; BORDER-LEFT: windowtext 1pt solid; COLOR: black; PADDING-TOP: 0pt; BORDER-BOTTOM: windowtext 1pt solid; FONT-FAMILY: Courier New"><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; <SPAN style="COLOR: blue">for</SPAN> (<SPAN style="COLOR: blue">int</SPAN> i = 0; i &lt; 10; i++)</PRE><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; {</PRE><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; Console.WriteLine(i.ToString());</PRE><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; }</PRE></DIV> <P>This above example outputs a list of numbers 0 through 9. And at times we need to loop through one variable (like i in the above example) yet increment another counter variable. So we do something like the below example:</P> <P><!--EndFragment--></P> <DIV style="BORDER-RIGHT: windowtext 1pt solid; PADDING-RIGHT: 0pt; BORDER-TOP: windowtext 1pt solid; PADDING-LEFT: 0pt; FONT-SIZE: 8pt; BACKGROUND: white; PADDING-BOTTOM: 0pt; BORDER-LEFT: windowtext 1pt solid; COLOR: black; PADDING-TOP: 0pt; BORDER-BOTTOM: windowtext 1pt solid; FONT-FAMILY: Courier New"><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; <SPAN style="COLOR: blue">int</SPAN> j = 0;</PRE><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; <SPAN style="COLOR: blue">for</SPAN> (<SPAN style="COLOR: blue">int</SPAN> i = 0; i &lt; 10; i++)</PRE><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; {</PRE><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; Console.WriteLine((j++).ToString());</PRE><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; }</PRE></DIV><!--EndFragment--> <P>Nothing wrong with this. It loops 10 times and increments j. This above snippet outputs a list of numbers 0 through 9. </P> <P>I recently was asked to debug some code that looked a little more like this:</P> <DIV style="BORDER-RIGHT: windowtext 1pt solid; PADDING-RIGHT: 0pt; BORDER-TOP: windowtext 1pt solid; PADDING-LEFT: 0pt; FONT-SIZE: 8pt; BACKGROUND: white; PADDING-BOTTOM: 0pt; BORDER-LEFT: windowtext 1pt solid; COLOR: black; PADDING-TOP: 0pt; BORDER-BOTTOM: windowtext 1pt solid; FONT-FAMILY: Courier New"><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; <SPAN style="COLOR: blue">int</SPAN> k = 0;</PRE><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; <SPAN style="COLOR: blue">for</SPAN> (<SPAN style="COLOR: blue">int</SPAN> i = 0; i &lt; 10; i++)</PRE><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; {</PRE><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; Console.WriteLine((++k).ToString());</PRE><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; }</PRE></DIV> <P>Again, it loops a finite number of times (10) and increments a separate counter variable (k in this case). But this time the out put is slightly different than the previous 2 examples. This code snippet outputs 1 - 10. The reason is obvious when you strip out all of the other code that was there already ... the incrementor (++) appears before the k in this example. Thus, k is incremented, then the ToString() method&nbsp;operates on it. In the previous example, j variable's value is output and THEN the incrementor (++) operates on the j variable. </P> <P>Not difficult to see in this case, of course. But the developer who was working on this was assured that x++ and ++x always responded the same, no matter the situation. Well, in MANY cases this is true. The above example could be modified so the incrementor preceeding or following the varialbe won't matter ... like either of these following code samples:</P> <DIV style="BORDER-RIGHT: windowtext 1pt solid; PADDING-RIGHT: 0pt; BORDER-TOP: windowtext 1pt solid; PADDING-LEFT: 0pt; FONT-SIZE: 8pt; BACKGROUND: white; PADDING-BOTTOM: 0pt; BORDER-LEFT: windowtext 1pt solid; COLOR: black; PADDING-TOP: 0pt; BORDER-BOTTOM: windowtext 1pt solid; FONT-FAMILY: Courier New"><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; <SPAN style="COLOR: blue">int</SPAN> x = 0;</PRE><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; <SPAN style="COLOR: blue">for</SPAN> (<SPAN style="COLOR: blue">int</SPAN> i = 0; i &lt; 10; i++)</PRE><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; {</PRE><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; Console.WriteLine(x.ToString());</PRE><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; x++;</PRE><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; }</PRE><PRE style="MARGIN: 0px">&nbsp;</PRE><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; <SPAN style="COLOR: blue">int</SPAN> y = 0;</PRE><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; <SPAN style="COLOR: blue">for</SPAN> (<SPAN style="COLOR: blue">int</SPAN> i = 0; i &lt; 10; i++)</PRE><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; {</PRE><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; Console.WriteLine(y.ToString());</PRE><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; ++y;</PRE><PRE style="MARGIN: 0px">&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; }</PRE></DIV><!--EndFragment--> <P>Both of these samples output 0-9 ... <STRONG>and both of these are much easier to read and less apt to wreak havoc than the previous inline examples</STRONG>.</P> <P>OK, I am running out of letters for examples, gotta run!</P>
