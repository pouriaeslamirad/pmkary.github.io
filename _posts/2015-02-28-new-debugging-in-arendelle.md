---
layout: post
title: New Debugging in Arendelle
---

![](http://kary.us/Graphics/Blog/6991.19.01.21/desk.png)

From now on you can debug your Arendelle code for real. Before this we had a system that enabled you to change title in your screen, All by writing a string there as <code class="arendelle">"some string"</code> and done! You had your title changed to `some string` and you know that we also had this great rich string interpolation there where you could write something in `\( ... )` of the string like <code class="arendelle">"1 + 2 = \\( 1 + 2 )"</code> and you got the title `1 + 2 = 3`. Now we thought hey! Why don't we collect all the title changes somewhere so you can use title changing as a kind of debugging console? So let's look my favorite example of Arendelle Arrays by writing my Fibonacci sequence from 1 to 100:

<pre class="arendelle">( f , 1; 1 )

[ 98 ,

	( f[ @f? ] , @f[ @f? - 1 ] + @f[ @f? - 2 ] )

	"Fibonacci at index: \( @f? ) is: \( @f[ @f? - 1 ] )"
]
</pre>

If you're using [Swifty](https://github.com/arendelle/swifty) there is the feature there as you can see in the image. And it will be there for Android and iOS too, Very soon!