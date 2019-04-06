---
layout: post
title: My experience with MacOs after switching from Linux/Windows
tags: [linux, mac, macOS, rant, productivity]
comments: true
---

__Notice:__ If you have never used Linux/Windows this post might be completely useless for you.  
MacOs is a good OS but it still has some serious issue from UX point of view if someone is coming from Linux/Windows background. Most of them aren't even better design choices. They are there just to make transition from MacOs to other platforms difficult. People who've never stepped out of Apple ecosystem will never notice that.  
For the folks going other way round it's not an adaptability issue, it about not having the features/functionality that could have been there but feels like intentionally omitted. MacOs is full of these half baked features that I'll be pointing out in this article one by one.  
Finally I'd like point out that this post is about my pet peeves and those are quite esoteric. You may not find yourself in the same shoes even if you are coming from Linux/Windows background.  

__PS:__ I am using a 2018 MacBook Pro model with 32GiB Ram.  

1. __Pseudo Delete Key:__ This is not a big issue but it's actually a _Backspace_ key labeled as _Delete_. Though they have extended its usage via some key combinations e.g. __cmd + delete__ will delete an item. For actual delete action you have to use __fn + delete__ combination.

2. __Can't close lid without putting mac to sleep:__ This is quite infuriating when you just want to play YouTube/Spotify in background and don't want the lid to be opened. I have tried my level best to search for an option where I can disable sleep if I close the lid but I never found one. Though there are some third party apps which can do this but seriously Apple, is it that hard? Please comment if you know how to solve this problem without installing a third party app.

3. __Delay when releasing the double-tap action on touchpad:__ For this to experience, you will need to enable __double tap to drag__ option first with locking disabled. This is like same good old feature where a user can double tap on touch pad to drag things around and releases the finger to stop the action. In Mac everything works fine except the part where you release the finger. Where it takes considerable chunk of time that it has become quite annoying for me. The consequence of this is that even if a user has released the finger the drag action will linger for some time in the UI and as soon as the user will try to move the pointer, it'll perform the drag action. I can't see why there is no way to set the release delay to zero. 

4. __No middle mouse button gesture in touchpad:__ I am a big fan of using middle mouse button. Especially for the feature like opening links in new tab and closing the tab in different applications like _Sublime Text_, _Google Chrome_ etc. On Windows/Linux you can map middle mouse button to triple finger tap on touchpad but for some reasons on Mac you can't, even though if you attach a mouse with middle button it understands that action. Right now I'm using a third party application _Middle Click_ to perform this gesture.

Further points are about Desktop feature in Mac. I will compare this feature to what I've already used in Linux i.e. [__i3 window manager__](https://en.wikipedia.org/wiki/I3_(window_manager)). Mac has desktop feature where you can create multiple desktops according to your own need. But unfortunately this is quite useless for the folks who actually want to use this feature for the reasons listed below.

5. __Command+Tab and Desktop feature:__ Suppose you have three desktops 1,2 and 3. Right now you are in desktop 3 and previously you were in desktop 1. Now if you'll press _cmd + tab_ for switching to an application which is in desktop 1, instead of jumping to desktop 1, Mac will simply move the desktop 1 to position 2. The problem here may not be obvious but if you use _ctrl + number_ to switch to a particular desktop, you'll find the shortcut useless. The funny part is that you can choose to assign desktop numbers to applications so that an application will be opened in a specific desktop only but Mac won't honor that setting if you'll press _cmd + tab_ shortcut.

6. __Switching apps in same desktop:__ Right now there is no way to switch applications in the same desktop. If you'll press the _cmd + tab_ shortcut you'll have to juggle your way through with bunch of other apps before finding the right one. This is not how you handle multiple desktops Apple. This actually defeats the purpose of having multiple desktop in the first place.

7. __No way to switch desktops back and forth:__ Currently there is a shortcut _ctrl + number_ using which you can quickly switch between desktops. But for example if you want to switch between desktops __1__ and __4__ quickly, you have to use the shortcut with the right desktop number. If you are wondering what would be the better design choice then I can give _i3's_ example, where for the same scenario you can use the shortcut with the same desktop number and it'll take you to the previous desktop. 

8. __Opening links from other apps:__ This is the issue that single handedly obliterates whatever desktop capability Mac has. If you'll try to open a link from some application other than your browser, Mac will simply pull the desktop which contains the browser next to the desktop from where you opened the link. And in doing so it'll also disrupt the order of all other desktops. So _ctrl + number_ will become instantly useless. And you have to manually order the desktops again if you want to use the _ctrl + number_ shortcut.


Those are some of the pet peeves that I seriously want Apple to address. Meanwhile if you guys have some solutions to the problems listed above please comment down. You can comment down your problems with Mac also, may be I'll be able to answer.