---
layout: page
title: Arendelle Coding Styles
---

When I made Arendelle I had this idea to make it’s language beautiful in design and when I say that I’m not mentioning the advances in technology but the code’s look itself. 

In it’s design I applied a very simple concept that I care so much and it’s use of spaces. I’ve seen programmers who agree with me. For example in the 125th issue of ACCU’s Overload there’s an article called “I Like Whitespace” which is also [available online here](http://accu.org/index.php/journals/2063)

I don’t agree with all other people’s ideas and for example i like the idea of CamelCase and camelBack naming styles and till this day I always hated underlines in names. So I will explain you how to code in my style with Arendelle however as every documentation of Arendelle till this day is written by me only way you may know of Arendelle codes are most probably my way however I would like ver much to once and for all explain how my style and notation works (Have in mind that this Arendelle’s original way of coding is what I show you here)

## Let’s start from basics
First thing you write in Arendelle is commands and we write commands with no space like this

```
prpldp
```

However sometime we separate this command with spaces like this:

```
prp ld prp
```

This kind of spacings gives `pro` and `ld` some kind of identity  which is very good when you’re going to read the codes. No when it comes to comments you may wonder how to space? In the other languages you do something like this which is really not cool:

```Objective-C
// allocing and initializing a string
NSString * str = [[NSString alloc] initWithString:@"Hello, World"];
```

In the time many people showed that `//` is not really pretty so they did this:

```Objective-C
//
// Allocing and initializing a string
//

NSString * str = [[NSString alloc] initWithString:@"Hello, World"];
```

In many Markdown editors like [iA Writer](http://www.iawriter.com) and [UberWriter](http://uberwriter.wolfvollprecht.de) you see this kind of highlighting:

![](http://kary.us/Graphics/Blog/6974.19.1.4/writer.png)

Which when you use `#` header operator it actually puts it out of the screen. I wanted such thing in the Arendelle so I comment like this:


<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->

<pre style="font-weight:bold; font-family: Menlo, Monaco, 'Courier 10 Pitch', Monospace;">
<span style="color: #A0A0A0;">//&nbsp;When&nbsp;you&nbsp;write&nbsp;comments&nbsp;things&nbsp;that&nbsp;are</span><br><span style="color: #A0A0A0;">//&nbsp;for&nbsp;the&nbsp;comment&nbsp;will&nbsp;come&nbsp;in&nbsp;3&nbsp;spaces&nbsp;so&nbsp;the</span><br><span style="color: #A0A0A0;">//&nbsp;like&nbsp;it’s&nbsp;part&nbsp;of&nbsp;the&nbsp;text’s&nbsp;content&nbsp;not&nbsp;`//&nbsp;`</span><br>&nbsp;&nbsp;&nbsp;<span style="color: #D60073;">[</span>&nbsp;<span style="color: #6200A8;">10</span>&nbsp;<span style="color: #D60073;">,</span>&nbsp;pr&nbsp;<span style="color: #D60073;">]</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->


This way you give the `// ` kind of a new life and a new look. Then what come to the mind is nested comments which is like vise:


<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->

<pre style="font-weight:bold; font-family: Menlo, Monaco, 'Courier 10 Pitch', Monospace;">
<span style="color: #A0A0A0;">//&nbsp;level&nbsp;one&nbsp;comment</span><br>&nbsp;&nbsp;&nbsp;<span style="color: #D60073;">[</span>&nbsp;<span style="color: #6200A8;">10</span>&nbsp;<span style="color: #D60073;">,</span>&nbsp;pr&nbsp;<span style="color: #D60073;">]</span><br><br>&nbsp;&nbsp;&nbsp;<span style="color: #A0A0A0;">//&nbsp;level&nbsp;two&nbsp;comment</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #D60073;">[</span>&nbsp;<span style="color: #6200A8;">20</span>&nbsp;<span style="color: #D60073;">,</span>&nbsp;pr&nbsp;<span style="color: #D60073;">]</span><br><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #A0A0A0;">//&nbsp;level&nbsp;three&nbsp;comment</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #D60073;">[</span>&nbsp;<span style="color: #6200A8;">10</span>&nbsp;<span style="color: #D60073;">,</span>&nbsp;pr&nbsp;<span style="color: #D60073;">]</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #D60073;">[</span>&nbsp;<span style="color: #6200A8;">10</span>&nbsp;<span style="color: #D60073;">,</span>&nbsp;pd&nbsp;<span style="color: #D60073;">]</span><br><br>&nbsp;&nbsp;&nbsp;<span style="color: #A0A0A0;">//&nbsp;back&nbsp;to&nbsp;level&nbsp;two</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #D60073;">[</span>&nbsp;<span style="color: #6200A8;">10</span>&nbsp;<span style="color: #D60073;">,</span>&nbsp;pr&nbsp;<span style="color: #D60073;">]</span><br><br><span style="color: #A0A0A0;">//&nbsp;done</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->


## Writing Grammars
In Arendelle all the grammars are same in design. All of the start with something and then you separate the parts using `,` and then they finish with something like

```
[ , ]  { , }  < , >  ( , ) 
```

And the format for highlighting this codes are simple. You should do this:

<br>
<img src="http://kary.us/Graphics/Blog/6974.19.1.4/spacingOf10pr.png/" style="width:18.9rem">
<br>

So I think I don’t have to guide you any more on this! Write things like:


<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->

<pre style="font-weight:bold; font-family: Menlo, Monaco, 'Courier 10 Pitch', Monospace;">
<span style="color: #D60073;">[</span>&nbsp;<span style="color: #6200A8;">10</span>&nbsp;<span style="color: #D60073;">,</span>&nbsp;pr&nbsp;<span style="color: #D60073;">]</span>&nbsp;ll&nbsp;<span style="color: #D60073;">[</span>&nbsp;<span style="color: #6200A8;">20</span>&nbsp;<span style="color: #D60073;">,</span>&nbsp;pr&nbsp;<span style="color: #D60073;">]</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->


## Mathematical Expressions
I believe if we write mathematical expressions with a space between all the operators like:


<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->

<pre style="font-weight:bold; font-family: Menlo, Monaco, 'Courier 10 Pitch', Monospace;">
<span style="color: #4E00FC;">@space</span>&nbsp;+&nbsp;<span style="color: #6200A8;">10</span>&nbsp;/&nbsp;<span style="color: #6200A8;">2</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->


Now the thing that comes to mind is parentheses. Apply the same principles on them as what we did before:


<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->

<pre style="font-weight:bold; font-family: Menlo, Monaco, 'Courier 10 Pitch', Monospace;">
<span style="color: #D60073;">(</span>&nbsp;<span style="color: #4E00FC;">#i</span>&nbsp;+&nbsp;<span style="color: #6200A8;">2</span>&nbsp;<span style="color: #D60073;">)</span>&nbsp;/&nbsp;<span style="color: #6200A8;">5</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->


You see how more clear they looks? You can also use them like:

```
( ( #i / 2 ) + 4 )
```

Speaking of parentheses when you use inline string replacers like:


<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->

<pre style="font-weight:bold; font-family: Menlo, Monaco, 'Courier 10 Pitch', Monospace;">
<span style="color: #BD00AD;">'Inline string replacer: </span><span style="color: #000000;">\(</span>&nbsp;<span style="color: #4E00FC;">@space</span>&nbsp;<span style="color: #000000;">)</span><span style="color: #BD00AD;">'</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->


Use a space before and after the math expression like:

<br>
<img src="http://kary.us/Graphics/Blog/6974.19.1.4/inSpaceStringReplacer.png/" style="width:21.5rem">
<br>


So with that do:


<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->

<pre style="font-weight:bold; font-family: Menlo, Monaco, 'Courier 10 Pitch', Monospace;">
<span style="color: #BD00AD;">'half of space is </span><span style="color: #000000;">\(</span>&nbsp;<span style="color: #4E00FC;">@space</span>&nbsp;/&nbsp;<span style="color: #6200A8;">2</span>&nbsp;<span style="color: #000000;">)</span><span style="color: #BD00AD;">'</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->


## Names
In Arendelle you can give **Spaces**, **Stored Spaces** and **Functions** names. naming this things are more often a very simple task like:


<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->

<pre style="font-weight:bold; font-family: Menlo, Monaco, 'Courier 10 Pitch', Monospace;">
<span style="color: #D60073;">(</span><span style="color: #4E00FC;">&nbsp;size&nbsp;</span><span style="color: #D60073;">,</span>&nbsp;<span style="color: #6200A8;">10</span>&nbsp;<span style="color: #D60073;">)</span>&nbsp;<span style="color: #D60073;">(</span>&nbsp;age&nbsp;<span style="color: #D60073;">,</span>&nbsp;<span style="color: #6200A8;">18</span>&nbsp;<span style="color: #D60073;">)</span>&nbsp;<span style="color: #D60073;">(</span>&nbsp;year&nbsp;<span style="color: #D60073;">,</span>&nbsp;<span style="color: #6200A8;">2015</span>&nbsp;<span style="color: #D60073;">)</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->


Space names are `lowercase` (`a-z` not `A-Z`) very simple. However the problem starts when you have more than one word for the name like


<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->

<pre style="font-weight:bold; font-family: Menlo, Monaco, 'Courier 10 Pitch', Monospace;">
<span style="color: #D60073;">(</span><span style="color: #4E00FC;">&nbsp;aLongName&nbsp;</span><span style="color: #D60073;">,</span>&nbsp;<span style="color: #6200A8;">10</span>&nbsp;<span style="color: #D60073;">)</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->


Like many implementations of FOTRAN, Arendelle removes all the new lines, spaces and tabs except the ones in strings prior to compile. So it really doesn't matter if you use spaces in the names 


<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->

<pre style="font-weight:bold; font-family: Menlo, Monaco, 'Courier 10 Pitch', Monospace;">
<span style="color: #D60073;">(</span><span style="color: #4E00FC;">&nbsp;age&nbsp;</span>of&nbsp;kary&nbsp;<span style="color: #D60073;">,</span>&nbsp;<span style="color: #6200A8;">19</span>&nbsp;<span style="color: #D60073;">)</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->


Is acceptable and well you can use it likewise as:


<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->

<pre style="font-weight:bold; font-family: Menlo, Monaco, 'Courier 10 Pitch', Monospace;">
<span style="color: #D60073;">[</span>&nbsp;<span style="color: #4E00FC;">@age</span>&nbsp;of&nbsp;kary&nbsp;<span style="color: #D60073;">,</span>&nbsp;<span style="color: #6200A8;">19</span>&nbsp;<span style="color: #D60073;">]</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->


As well as using


<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->

<pre style="font-weight:bold; font-family: Menlo, Monaco, 'Courier 10 Pitch', Monospace;">
<span style="color: #D60073;">[</span>&nbsp;<span style="color: #4E00FC;">@ageOfKary</span>&nbsp;<span style="color: #D60073;">,</span>&nbsp;<span style="color: #6200A8;">19</span>&nbsp;<span style="color: #D60073;">]</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->


Thanks to these `@`, `#`, `!`, `$` Arendelle won't read the name wrong so there are some very common popular rules in space naming like `CamelCase`, `camelBack` and `using_underscore_as_whitespace` like

```C
ageOfKary   // camelBack
AgeOfKary   // CamelCase
age_of_kary // underscores
```

But when you can use spaces in Arendelle why not? You can do:


<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->

<pre style="font-weight:bold; font-family: Menlo, Monaco, 'Courier 10 Pitch', Monospace;">
<span style="color: #D60073;">(</span><span style="color: #4E00FC;">&nbsp;age&nbsp;</span>of&nbsp;kary&nbsp;<span style="color: #D60073;">,</span>&nbsp;<span style="color: #6200A8;">19</span>&nbsp;<span style="color: #D60073;">)</span>&nbsp;<span style="color: #D60073;">[</span>&nbsp;<span style="color: #4E00FC;">@age</span>&nbsp;of&nbsp;kary&nbsp;<span style="color: #D60073;">,</span>&nbsp;pr&nbsp;<span style="color: #D60073;">]</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->


When it comes to `!`, `@`, `$`, `#` and `.` for directory addressing use them like this:


<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->

<pre style="font-weight:bold; font-family: Menlo, Monaco, 'Courier 10 Pitch', Monospace;">
<span style="color: #D60073;">(</span>&nbsp;<span style="color: #4E00FC;">$stored</span>&nbsp;space&nbsp;<span style="color: #D60073;">,</span>&nbsp;<span style="color: #6200A8;">10</span>&nbsp;<span style="color: #D60073;">)</span>&nbsp;<span style="color: #D60073;">[</span>&nbsp;<span style="color: #4E00FC;">@space</span>&nbsp;name&nbsp;<span style="color: #D60073;">,</span>&nbsp;pr&nbsp;<span style="color: #D60073;">]</span>&nbsp;<br><span style="color: #D60073;">[</span>&nbsp;<span style="color: #4E00FC;">@use</span>&nbsp;.of&nbsp;.stored&nbsp;space&nbsp;<span style="color: #D60073;">,</span>&nbsp;pr&nbsp;<span style="color: #D60073;">]</span>&nbsp;<br></pre>

<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->


If you're a developer like me this kind of naming may look a bit strange and confusing to you. I know at first it's unacceptable but as soon as you worm up to it, It becomes a more readable way to read and write codes.

And if you didn't well you're still free to do what ever you want! 

## Functions
I very much like to write function names like this:


<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->

<pre style="font-weight:bold; font-family: Menlo, Monaco, 'Courier 10 Pitch', Monospace;">
<span style="color: #D60073;">!func</span>&nbsp;name&nbsp;<span style="color: #D60073;">(</span><span style="color: #D60073;">)</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->


And also function address:


<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->

<pre style="font-weight:bold; font-family: Menlo, Monaco, 'Courier 10 Pitch', Monospace;">
<span style="color: #D60073;">!folder</span>&nbsp;.func&nbsp;<span style="color: #D60073;">(</span><span style="color: #D60073;">)</span>&nbsp;<span style="color: #A0A0A0;">/*&nbsp;or&nbsp;*/</span>&nbsp;<span style="color: #D60073;">!folder.func</span>&nbsp;<span style="color: #D60073;">(</span><span style="color: #D60073;">)</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->


## Multi Line Comments
Use the C way, However after stating asterisks use 3 spaces, Something like this:


<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->

<pre style="font-weight:bold; font-family: Menlo, Monaco, 'Courier 10 Pitch', Monospace;">
<span style="color: #A0A0A0;">/*<br>&nbsp;&#42;&nbsp;&nbsp;&nbsp;A&nbsp;multi&nbsp;line<br>&nbsp;&#42;&nbsp;&nbsp;&nbsp;comment&nbsp;must&nbsp;be&nbsp;something<br>&nbsp;&#42;&nbsp;&nbsp;&nbsp;very&nbsp;much&nbsp;like&nbsp;this<br>&nbsp;*/</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->


## Arrays
It's better if you init multi member arrays like this:


<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->

<pre style="font-weight:bold; font-family: Menlo, Monaco, 'Courier 10 Pitch', Monospace;">
<span style="color: #D60073;">(</span><span style="color: #4E00FC;">&nbsp;array&nbsp;</span><span style="color: #D60073;">,</span>&nbsp;<span style="color: #6200A8;">12</span><span style="color: #D60073;">;</span>&nbsp;<span style="color: #6200A8;">23</span><span style="color: #D60073;">;</span>&nbsp;<span style="color: #6200A8;">34</span><span style="color: #D60073;">;</span>&nbsp;<span style="color: #6200A8;">454</span><span style="color: #D60073;">;</span>&nbsp;<span style="color: #6200A8;">232</span>&nbsp;<span style="color: #D60073;">)</span>&nbsp;<br></pre>

<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->


And please no:


<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->

<pre style="font-weight:bold; font-family: Menlo, Monaco, 'Courier 10 Pitch', Monospace;">
<span style="color: #D60073;">(</span><span style="color: #4E00FC;">array</span><span style="color: #D60073;">,</span><span style="color: #6200A8;">23</span><span style="color: #D60073;">;</span>&nbsp;<span style="color: #6200A8;">23</span><span style="color: #D60073;">;</span><span style="color: #6200A8;">34</span><span style="color: #D60073;">;</span>&nbsp;<span style="color: #6200A8;">23</span><span style="color: #D60073;">;</span><span style="color: #6200A8;">2122</span><span style="color: #D60073;">)</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->


Also when you want to load an array index use this way:


<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->

<pre style="font-weight:bold; font-family: Menlo, Monaco, 'Courier 10 Pitch', Monospace;">
<span style="color: #4E00FC;">@array</span><span style="color: #D60073;">[</span>&nbsp;<span style="color: #4E00FC;">@index</span>&nbsp;<span style="color: #D60073;">]</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->


Also for nested ones use:


<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->

<pre style="font-weight:bold; font-family: Menlo, Monaco, 'Courier 10 Pitch', Monospace;">
<span style="color: #4E00FC;">@array</span><span style="color: #D60073;">[</span>&nbsp;<span style="color: #4E00FC;">@nested</span>&nbsp;array<span style="color: #D60073;">[</span>&nbsp;<span style="color: #4E00FC;">@also</span>&nbsp;nested&nbsp;array<span style="color: #D60073;">[</span>&nbsp;<span style="color: #4E00FC;">@index</span>&nbsp;<span style="color: #D60073;">]</span>&nbsp;<span style="color: #D60073;">]</span>&nbsp;<span style="color: #D60073;">]</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->


## Nested grammars. 
As I said before use 3 space tabs and this style:


<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->

<pre style="font-weight:bold; font-family: Menlo, Monaco, 'Courier 10 Pitch', Monospace;">
<span style="color: #D60073;">(</span><span style="color: #4E00FC;">&nbsp;line&nbsp;</span><span style="color: #D60073;">,</span>&nbsp;<span style="color: #6200A8;">0</span>&nbsp;<span style="color: #D60073;">)</span><br><span style="color: #D60073;">[</span>&nbsp;<span style="color: #4E00FC;">#j</span><span style="color: #D60073;">,</span><br>&nbsp;&nbsp;&nbsp;&nbsp;i&nbsp;<span style="color: #D60073;">[</span>&nbsp;<span style="color: #4E00FC;">@line</span>&nbsp;<span style="color: #D60073;">,</span>&nbsp;d&nbsp;<span style="color: #D60073;">]</span>&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #D60073;">(</span><span style="color: #4E00FC;">&nbsp;line&nbsp;</span><span style="color: #D60073;">,</span>&nbsp;+<span style="color: #6200A8;">1</span>&nbsp;<span style="color: #D60073;">)</span><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: #D60073;">{</span>&nbsp;<span style="color: #4E00FC;">#x</span>&nbsp;<span style="color: #D60073;"><</span>&nbsp;<span style="color: #4E00FC;">#y</span>&nbsp;<span style="color: #D60073;">,</span>&nbsp;p&nbsp;<span style="color: #D60073;">}</span>&nbsp;r<br><span style="color: #D60073;">]</span><br></pre>

<!-- CLIFF HIGHLIGHTER 0.05 DEV GENERATED CODE BLOCK-->


I think that was a good enough example!

<br><br><br>

# That's it!
I hope you like my style of coding. This is the actual way that Arendelle is made for and I hope you use it too. A part of my style is using **First Spacings**, **Standard Copyright** and **Done** comment which that are explained in the [Arendelle Book](http://web.arendelle.org/book). So I hope you use them too. Also gimme your suggestions on how to make this style better.
