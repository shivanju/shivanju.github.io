---
layout: post
title: Apps for de-googling your phone
tags: [android, google, opensource, applications]
comments: true
---

Six months ago I thought of doing an experiment. It was getting rid of most of the of the default applications that came pre-installed with my android phone and trying out their alternatives. And not only for default apps but also for some other popular applications like Lastpass. The alternative may be primarily open source or proprietary. Since most of the default apps are provided by Google, you can say this experiment was sort of de-googling my phone.  

It's been more than six months after de-googling my phone and I don't think I'm going to revert it. This article is also helpful for those people who are concerned about Google storing their data as most of the applications are open source and they don't store any kind of data.  

It can be hard for some people to uninstall the default apps entirely and as a result of this they might feel reluctant to try out alternatives. No one wants to have two apps for the same purpose. Still I would say try and then uninstall it. For folks out there who can get their hands dirty I would say that try de-googling your phone for few days and see whether you like it or not. It might take some days to get accustom to this change but after that you won't feel much of a difference.  

Now about my setup. I have a rooted Moto G5 Plus with [AEX][aex] Oreo installed along with the playstore(the only Google app) which might come handy sometimes. I am using it as my daily driver from last six months. Below I have listed down some applications and their alternatives along with the project page incase you want to contribute.  

#### __Playstore__:
__[F-Droid][fdroid]__: This is basically the Playstore of opensource apps. This is one of the first app that you should install if you want to automatically update your apps that are not from playstore.

#### __Google Chrome__:
__[Firefox][firefox]__: No introduction needed here. It's in the market for more than 15 years. Earlier I was reluctant to switch to Firefox but recent updates made web-page rendering smoother and faster. Another feature is that Firefox lets you install extensions whereas Chrome doesn't. Though performance wise it's still slightly behind Chrome but it's not that much noticeable.

#### __YouTube__:
__[NewPipe][newpipe]__: So far this is the best alternative I've ever used and that too better than original. It's an android app wrapper on top of YouTube's website. It has everything that YouTube has and apart from that it has some awesome features like background play, pop-up player and audio/video download. There is one caveat though that you can't sign-in to YouTube, but that should have been obvious till now. That means no sync feature either. Still you can import you existing subscriptions by following the simple procedure described in the app.

#### __Offline Multimedia Player__:
__[VLC][vlc]__: This shouldn't be a new name for you. Like it's desktop variant, VLC-android has all the features in one package. You may find some fancy music players in playstore but VLC beats them all without a doubt. It has audio/video player together. It even has a stream player, so just input a YouTube URL and start playing.

#### __Google Maps__:
__[OsmAnd][osmand]__: Osm (Open Street Map) is a quite good alternative but still lacks the experience the G-maps provide  as a whole. Ultimately it depends on the community that uses and contributes to it. As the number of users/contributors will increase so does the quality of Osm.  
Another alternative which is not open source is __[Here maps][heremaps]__. Though the map is not as detailed as G-maps but usually it's not a problem unless you are in some remote area.  
Not to mention that in the worst case if you have to use G-maps you can always open it in your browser. There will be some latency in updating your live location but it will do the job.

#### __Gmail Client__:
__[K-9 Mail][k9mail]__: K-9 is a slim and fast alternative to Gmail client. It doesn't have a
sleek UI like Gmail but functionally it has everything that one might expect from an email client. One downside of K-9 is that it doesn't have [ActiveSync][activesync] support because it's a proprietary protocol developed by Microsoft. So if you are one of those who needs ActiveSync support, hard luck here.  
__[BlueMail][bluemail]__ is another email client that doesn't have the previously mentioned issue. Though it comes at a cost. Bluemail is not opensource. One good side is that it's free(of cost) and ad free. Though you might want to have look at their [privacy policy][bluemail_policy].

#### __Gmail Service__:
__[ProtonMail][protonmail]__: There are lot of email service provider in the market and there is an option to host for yourself. Protonmail is the one which has stuck to me for past six months. It's open source, has it's own client and supports [PGP][pgp]. It has different tiers of subscriptions. I use free tier which has 500 MB of free storage, 3 custom folders and 3 custom labels. 500 MB might sound less but from past six months my inbox hasn't even reached 60 MB. And that too when I have switched all of my accounts on different sites to Protonmail.  
Other alternatives are also available in the market such as __[FastMail][fastmail]__, __[HushMail][hushmail]__, __[MailFence][mailfence]__ etc. You can give them a try and see what you like most and which service is best suited for your needs. 

#### __Google Keep__:
__[Orgzly][orgzly]__: This is not like any other note taking app. It is an implementation of [Org mode][orgmode] for android. If you are familiar with the Orgmode, it's good, else the app itself comes with the starting guide note which will explain everything in detail. This app has everything that you can expect from a good note taking app such as checkboxes, ToDo, reminders, nested notes, notebooks and even syncing across devices. For backup and syncing you have two options, either save it locally or in Dropbox.


#### __Google Authenticator__:
__[andOTP][andotp]__: An open source project for generating OTPs locally. Simply does what it says. It has sleek UI, password/pin protection and encrypted backup support.

#### __Backup and Sync__:
__[Syncthing][syncthing]__: As you might have noticed till now that some of the apps mentioned above doesn't have their own backup/sync feature. Syncthing mitigates this limitation by providing a universal backup and sync mechanism. Since it's a peer to peer solution your data will be with you and you only. No servers or 3rd party service is involved. All you had do is to run syncthing on all the devices where you want your data to be synced, select the directories you want to sync and you are done. Since it's p2p it can even work without internet given that your devices are in the same network.

#### __Lastpass__:
__[Bitwarden][bitwarden]__: Another password manager like Lastpass but open source and an option to host your own server if you don't like using their servers. It has clients for every platform you can imagine be it mobile, desktop or browsers.  
Personally I don't use any password manager, I have my own little scripts which do the job for me. But if I had to it would be bitwarden for now.


Those are the some apps that you might want to try. You can either take the route that I took or cherry pick the apps that you like. You can also comment down if I missed some app that you think should belong here. I'll keep updating this space with newer/better alternatives. My main motive for writing this article was to spread the awareness that there are some good alternatives available that are not so popular but worth trying.  

[fdroid]: https://f-droid.org/
[firefox]: https://www.mozilla.org/en-US/firefox/mobile/
[aex]: https://forum.xda-developers.com/g5-plus/development/rom-aospextended-rom-v5-0-t3687007
[newpipe]: https://newpipe.schabi.org/
[vlc]: https://www.videolan.org/vlc/download-android.html
[osmand]: http://osmand.net
[heremaps]: https://wego.here.com/
[k9mail]: https://k9mail.github.io/
[protonmail]: https://protonmail.com/
[bluemail]: https://bluemail.me/
[bluemail_policy]: https://bluemail.me/privacy/
[activesync]: https://en.wikipedia.org/wiki/Exchange_ActiveSync
[pgp]: https://en.wikipedia.org/wiki/Pretty_Good_Privacy
[fastmail]: https://www.fastmail.com/
[hushmail]: https://www.hushmail.com/
[mailfence]: https://mailfence.com/
[orgzly]: http://www.orgzly.com/
[orgmode]: https://orgmode.org/
[andotp]: https://github.com/andOTP/andOTP
[syncthing]: https://syncthing.net/
[bitwarden]: https://bitwarden.com/