---
layout: page
title: Arendelle Coding Style
---

When I made Arendelle I had this idea to make it’s language beautiful in design and when I say that I’m not mentioning the advances in technology but the code’s look itself. 

In it’s design I applied a very simple concept that I care so much and it’s use of spaces. I’ve seen programmers who agree with me. For example in the 125th issue of ACCU’s Overload there’s an article called “I Like Whitespace” which is also [available online here](http://accu.org/index.php/journals/2063)

I don’t agree with all other people’s ideas and for example i like the idea of CamelCase and camelBack naming styles and till this day I always hated underlines in names. So I will explain you how to code in my style with Arendelle however as every documentation of Arendelle till this day is written by me only way you may know of Arendelle codes are most probably my way however I would like ver much to once and for all explain how my style and notation works (Have in mind that this Arendelle’s original way of coding is what I show you here)

<br><br>

## Let’s start from basics
First thing you write in Arendelle is commands and we write commands with no space like this

<pre class="arendelle">prpldp
</pre>

However sometime we separate this command with spaces like this:

<pre class="arendelle">prp ld prp
</pre>

This kind of spacings gives `prp` and `ld` some kind of identity  which is very good when you’re going to read the codes. No when it comes to comments you may wonder how to space? In the other languages you do something like this which is really not cool:

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

<br>
![](http://kary.us/Graphics/Blog/6974.19.1.4/writer.png)
<br>

Which when you use `#` header operator it actually puts it out of the screen. I wanted such thing in the Arendelle so I comment like this:

<pre class="arendelle">// When you write comments things that are
// for the comment will come in 3 spaces so the
// like it’s part of the text’s content not '// '
   [ 10 , pr ]</pre>

This way you give the `// ` kind of a new life and a new look. Then what come to the mind is nested comments which is like vise:


<pre class="arendelle">// level one comment
   [ 10 , pr ]

   // level two comment
        [ 20 , pr ]

      // level three comment
         [ 10 , pr ]
         [ 10 , pd ]

   // back to level two
      [ 10 , pr ]

// done</pre>

<br><br>

## Writing Grammars

In Arendelle all the grammars are same in design. All of the start with something and then you separate the parts using `,` and then they finish with something like:

<pre class="arendelle">[ , ]  { , }  &lt; , &gt;  ( , )</pre>

And the format for highlighting this codes are simple. You should do this:

<br><center>
<img src="http://kary.us/Graphics/Blog/6974.19.1.4/spacingOf10pr.png" style="width:18.9rem">
</center><br>

So I think I don’t have to guide you any more on this! Write things like:

<pre class="arendelle">[ 10 , pr ] ll [ 20 , pr ]</pre>

<br><br>
## Mathematical Expressions
I believe if we write mathematical expressions with a space between all the operators like:

<pre class="arendelle">@space + 10 / 2</pre>

Now the thing that comes to mind is parentheses. Apply the same principles on them as what we did before:

<pre class="arendelle">( #i + 2 ) / 5</pre>

You see how more clear they looks? You can also use them like:

<pre class="arendelle">( ( #i / 2 ) + 4 )</pre>

Speaking of parentheses when you use inline string replacers like:

<pre class="arendelle">'Inline string replacer: \( @space )'</pre>

Use a space before and after the math expression like:

<pre class="arendelle">'half of space is \( @space / 2 )'</pre>


<br><br>
## Names
In Arendelle you can give **Spaces**, **Stored Spaces** and **Functions** names. naming this things are more often a very simple task like:

<pre class="arendelle">( size , 10 )</pre>

Space names are `lowercase` (`a-z` not `A-Z`) very simple. However the problem starts when you have more than one word for the name like

<pre class="arendelle">( aLongName , 10 )</pre>

Like many implementations of FORTRAN, Arendelle removes all the new lines, spaces and tabs except the ones in strings prior to compile. So it really doesn't matter if you use spaces in the names 

<pre class="arendelle">( age of kary , 19 )</pre>

Is acceptable and well you can use it likewise as:

<pre class="arendelle">[ @age of kary , 19 ]</pre>

As well as using

<pre class="arendelle">[ @ageOfKary , 19 ]</pre>

Thanks to these `@`, `#`, `!`, `$` Arendelle won't read the name wrong so there are some very common popular rules in space naming like `CamelCase`, `camelBack` and `using_underscore_as_whitespace` like

```C
ageOfKary   // camelBack
AgeOfKary   // CamelCase
age_of_kary // underscores
```

But when you can use spaces in Arendelle why not? You can do:

<pre class="arendelle">( age of kary , 19 ) [ @age of kary , pr ]</pre>

When it comes to `!`, `@`, `$`, `#` and `.` for directory addressing use them like this:

<pre class="arendelle">( $stored space , 10 ) [ @space name , pr ] 
[ $use .of .stored space , pr ]</pre>

If you're a developer like me this kind of naming may look a bit strange and confusing to you. I know at first it's unacceptable but as soon as you worm up to it, It becomes a more readable way to read and write codes.

And if you didn't well you're still free to do what ever you want! 

<br><br>
## Functions
I very much like to write function names like this:

<pre class="arendelle">!func name ()</pre>

And also function address:

<pre class="arendelle">!folder .func () /* or */ !folder.func ()</pre>

Now when you're making libraries do this kind of coding style. I like it very much:

<pre class="arendelle">!math. floor ()</pre>

And sometimes:

<pre class="arendelle">!math.array. floor ()</pre>

Also something that is very important about functions is their special comments. To use function comments use this way:

<pre class="arendelle">!func ( init with number: 12, and number: 5 )</pre>

Write them lowercase and don't frogot the space after `(` and `,`. So like the example I showed you!

<br><br>
## Multi Line Comments
Use the C way, However after stating asterisks use 3 spaces, Something like this:

<pre class="arendelle">/*
 *   A multi line
 *   comment must be something
 *   very much like this
 */</pre>


But hey I hate this multi line comments! I have them in Arendelle because well they are C style and sometimes they are hany but when it comes tot he multi line comments use this system:

<pre class="arendelle">//
// A multi line
// comment must be something
// very much like this
//</pre>

As you see it's a much more beautiful way to wite comments, I use them most of the times for section flags like:

<pre class="arendelle">//
// BODY
//

   [ 10 , pr ]

//
// DONE
//</pre>

<br><br>
## Arrays
It's better if you init multi member arrays like this:

<pre class="arendelle">( array , 12; 23; 34; 454; 232 )</pre>

And please no:

<pre class="arendelle">(array,23; 23;34; 23;2122)</pre>

Also when you want to load an array index use this way:

<pre class="arendelle">@array[ @index ]</pre>

Also for nested ones use:

<pre class="arendelle">@array[ @nested array[ @also nested array[ @index ] ] ]</pre>

<br><br>
## Nested grammars. 
As I said before use 3 space tabs and this style:

<pre class="arendelle">( line , 0 )

[ #j,

    i [ @line , d ] 
    ( line , +1 )
    { #x < #y , p } r

]</pre>

I think that was a good enough example!

<br><br><br>

## That's it!
I hope you like my style of coding. This is the actual way that Arendelle is made for and I hope you use it too. A part of my style is using **First Spacings**, **Standard Copyright** and **Done** comment which that are explained in the [Arendelle Book](http://web.arendelle.org/book). So I hope you use them too. Also gimme your suggestions on how to make this style better.





