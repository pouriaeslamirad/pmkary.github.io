---
layout: post
title: I ♥︎ UNIX I
---

I love UNIX, It's the most beautiful system I've ever seen. It's clear, It's brilliant, It's a LEGO. You have some tools. You LEGO this tools tighter and you make something you want. You can script all your apps together… So much possibilities! So many of the UNIXians that I know write in their blogs why they love UNIX or some of them write especially for GNU/Linux. But I love UNIX and I'm going to write about UNIX!

If you're a UNIX fella you know that when you're scripting you can add this line in the top of your file:

```Bash
#!/usr/bin/env lua
```

To for example run a lua app by just running it's name like

```
% ./app.lua
```

And not

```
% lua ./app.lua
```

And so you can change the Lua to `python2` and use Python, You can change `python2` to `ruby` and so on. Well today I accidentally removed the `env` app in my system.

So I removed a system software that my life depends on it. So if it was Windows, I most certainly had to reinstall system and everything else I had. I mean they are native system files, You can just copy-paste them from another computer. Also you can't find any website to download `env`. As much as it looks scary it was the easiest problem I solved in my entire life. I just opened a web browser, Searched for `env` and turned out it's a part of 	*GNU CoreUtils*. So simply! I searched FSF's FTP and found the source bundle of coreutils. I compiled it with a typical

```
% configure
% make
```

Child's play. And then done, I had the `env`, So just a simple

```
% sudo mv ./env /usr/bin
```

And it was fixed, Just like the 3 mins earlier. So you know a problem like this could destroy my life in Windows and other non-unix platforms, But it's UNIX and even problems like this are the easiest when you wanna fix them. However if you're a Windows user you should never be worried about something like this. First because Windows is not this powerful to have useful tools! And also the simple fact that you have no right to understand and use the system utilities of your system! Ha Ha!