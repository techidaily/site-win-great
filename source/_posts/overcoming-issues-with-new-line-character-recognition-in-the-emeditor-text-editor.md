---
title: Overcoming Issues with New Line Character Recognition in the emEditor Text Editor
date: 2024-10-09T11:11:57.708Z
updated: 2024-10-11T15:05:55.502Z
tags:
  - product
categories:
  - emeditor
thumbnail: https://thmb.techidaily.com/1d662e9b1599361d80a888fd1a81a529179f95c0fe44fe20c4f91438bc57f9cb.jpg
---

## Overcoming Issues with New Line Character Recognition in the emEditor Text Editor

Viewing 4 posts - 1 through 4 (of 4 total)

* Author  
Posts
* August 24, 2011 at 2:48 pm [#9589](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/23d717965f2d4f3bb4f9f46094bedcd7?s=80&d=identicon&r=g)shellymeow](https://www.emeditor.com/forums/users/shellymeow/ "View shellymeow's profile")  
Member  
Hello everyone  
 Sorry about my poor English..  
 I already enabled _“Regular Expressions Match New Line Characters”_ checkbox  
 but I still cannot find out the string contains a new line that with the regular expression  
**.\*?**  
    
 why?  
 the version is 10.1.1  
August 24, 2011 at 4:52 pm [#9591](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/c962eeb8483fd8ad7d82a003f8405439?s=80&d=identicon&r=g)Deipotent](https://www.emeditor.com/forums/users/deipotent/ "View Deipotent's profile")  
Participant  
You also need to change the option below the “Regular Expressions Match New Line Characters” checkbox, “Additional Lines to Search for Regular Expressions”, from 0 to the maximum number of lines a tag could span. For example, if your tag is:  
    
	<td>first line  
	second line</td>  
	 you need to set it to 1, as the tag is one line later than the  
 tag. the higher the number you set it, the slower the regex engine will work, as it will be looking at more lines.  
 You could try setting to 100 or 1000 and see how performance is.  
August 24, 2011 at 5:05 pm [#9593](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/23d717965f2d4f3bb4f9f46094bedcd7?s=80&d=identicon&r=g)shellymeow](https://www.emeditor.com/forums/users/shellymeow/ "View shellymeow's profile")  
Member  
It works!!  
 Thank You so much!  
August 24, 2011 at 8:21 pm [#9601](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/f29c043a3cc5c5dac8db4e62939893e9?s=80&d=identicon&r=g)Stefan](https://www.emeditor.com/forums/users/Stefan/ "View Stefan's profile")  
Participant  
There could be an warning dialog after clicking \[OK\]  
**IF** “Regular Expressions Match New Line Characters” is checked  
**AND** “Additional Lines to Search for Regular Expressions” is set to ‘0’  
 Like:  
 “You have chosen to use RegEx in multi line mode.  
 Please note that you have to set the roughly expected “Additional Lines” option too.”  
 –  
 EDIT:  
 Or an better idea:  
 That two options could be somehow “grouped” by an thin frame line,  
 and the “Additional Lines” option could be greyed-out  
 while “Match New Line” is disabled,  
 to make the relationship better visible.  
 —————————————————  
 “\[X\] Regular Expressions Match New Line Characters”  
 “Multi Line mode search max. for \[0 \] additional lines.”  
 —————————————————  
 – – –  
 Or maybe these option could be set to an higher amount as ‘0’ by default.  
 Would be an amount of, lets say, ’30’ really that slow?  
 .
* Author  
Posts

Viewing 4 posts - 1 through 4 (of 4 total)

* You must be logged in to reply to this topic.

<ins class="adsbygoogle"
     style="display:block"
     data-ad-format="autorelaxed"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="1223367746"></ins>

<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="8358498916"
     data-ad-format="auto"
     data-full-width-responsive="true"></ins>

<span class="atpl-alsoreadstyle">Also read:</span>
<div><ul>
<li><a href="https://instagram-clips.techidaily.com/new-localizing-your-content-adding-subtitles-to-igtv-for-2024/"><u>[New] Localizing Your Content Adding Subtitles to IGTV for 2024</u></a></li>
<li><a href="https://tiktok-video-recordings.techidaily.com/updated-2024-approved-gamers-gauntlet-bizarre-tiktok-games-you-must-try/"><u>[Updated] 2024 Approved Gamer's Gauntlet Bizarre TikTok Games You Must Try</u></a></li>
<li><a href="https://fox-glue.techidaily.com/updated-in-2024-how-to-gently-lower-volume-without-distortion/"><u>[Updated] In 2024, How to Gently Lower Volume Without Distortion</u></a></li>
<li><a href="https://android-location-track.techidaily.com/in-2024-how-to-track-zte-axon-40-lite-location-by-number-drfone-by-drfone-virtual-android/"><u>In 2024, How to Track ZTE Axon 40 Lite Location by Number | Dr.fone</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/in-2024-how-to-unlock-sim-card-on-oneplus-ace-3-online-without-jailbreak-by-drfone-android/"><u>In 2024, How to Unlock SIM Card on OnePlus Ace 3 online without jailbreak</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/in-2024-the-magnificent-art-of-pokemon-go-streaming-on-lenovo-thinkphone-drfone-by-drfone-virtual-android/"><u>In 2024, The Magnificent Art of Pokemon Go Streaming On Lenovo ThinkPhone? | Dr.fone</u></a></li>
<li><a href="https://win-great.techidaily.com/master-the-art-of-video-harvesting-on-56com-at-no-charge/"><u>Master the Art of Video Harvesting on 56.com at No Charge</u></a></li>
<li><a href="https://win-great.techidaily.com/step-by-step-tutorial-on-transforming-babytv-streams-to-popular-file-types-such-as-mp3-mp4-and-more/"><u>Step-by-Step Tutorial on Transforming BabyTV Streams to Popular File Types Such as MP3, MP4, and More</u></a></li>
<li><a href="https://win-great.techidaily.com/step-by-step-tutorial-transforming-damasios-lecture-videos-to-compatible-mp4-and-mov-formats-across-windows-and-mac-systems/"><u>Step-by-Step Tutorial: Transforming Damasio's Lecture Videos to Compatible MP4 and MOV Formats Across Windows & Mac Systems</u></a></li>
<li><a href="https://extra-hints.techidaily.com/the-insiders-guide-to-snapchats-spotlight-feature/"><u>The Insider's Guide to Snapchat's Spotlight Feature</u></a></li>
<li><a href="https://win-great.techidaily.com/top-reliable-spotify-converters-for-pc-and-mac-a-comprehensive-guide-beyond-ondesoft/"><u>Top Reliable Spotify Converters for PC & MAC: A Comprehensive Guide Beyond Ondesoft</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2137378/7443" target="_top" id="2137378">
  <img src="//a.impactradius-go.com/display-ad/7443-2137378" border="0" alt="https://techidaily.com" width="600" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2137378/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

