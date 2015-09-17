---
layout: post
title: Silverlight Chord Finder
date: 2009-03-10 02:31
author: John
comments: true
categories: [Silverlight]
---
<p>I’ve been working on an article that features several aspects of building a Silverlight application. The article demonstrates data binding, some visual effects, effective resource use, playing audio files, creating states with the Visual State Manager and the CoolMenu from the <a href="http://silverlightcontrib.codeplex.com/">SilverlightContrib</a> project. The point of the article is to demonstrate these aspects, but I figured I might as well make the application fun to write. For this reason, I chose to use a chord finder as my sample application (see below). I decided to only show the first 5 frets of a guitar and use the major and minor scales. I’m going to post the source code for this on CodePlex once I run a few more tests and the article is published (hopefully within a week in time for <a href="http://2009.visitmix.com/">MIX09</a>). </p>  <p>Here is a quick look at the application, where a G major chord is being selected.</p>  <p>&#160;<a href="/wp-content/uploads/files/media/image/WindowsLiveWriter/SilverlightChordFinder_21E3/image_5.png"><img style="border-bottom: 0px; border-left: 0px; display: inline; border-top: 0px; border-right: 0px" title="image" border="0" alt="image" src="/wp-content/uploads/files/media/image/WindowsLiveWriter/SilverlightChordFinder_21E3/image_thumb_1.png" width="532" height="406" /></a> </p>  <p>One important disclaimer: I chose to use calculations to figure out how to play each chord. For the above G major chord, this works quite well. In fact, for most of the chords it works great. However when it comes to the B major chord, for example, the most common way to play a B chord is NOT what my calcs came up with (though its still correctly a B major chord). So there are 3 routes to take: (1) leave it as is (2) add additional logic to make the chords show the chord variations you desire or (3) remove the calculations and predefine the chord positions. I’ll explain more about this in the article. Once it is on CodePlex, I welcome any improvements.</p>  <p>And yes, the notes and chords being played are from me … an absolute beginner with the guitar. :)</p>
