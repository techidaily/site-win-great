---
title: Overcoming Issues with New Line Character Recognition in the emEditor Text Editor
date: 2024-11-19T02:41:20.920Z
updated: 2024-11-23T00:26:11.834Z
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
<li><a href="https://youtube-sure.techidaily.com/oost-viewers-interaction-via-youtube-cards-for-2024/"><u>[New] Boost Viewers Interaction via YouTube Cards for 2024</u></a></li>
<li><a href="https://article-knowledge.techidaily.com/updated-2024-approved-iphone-luminance-mastering-dark-imagery/"><u>[Updated] 2024 Approved IPhone Luminance Mastering Dark Imagery</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/updated-live-content-keepers-facebook-update/"><u>[Updated] Live Content Keepers - Facebook Update</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/3-methods-to-mirror-samsung-galaxy-m14-5g-to-roku-drfone-by-drfone-android/"><u>3 Methods to Mirror Samsung Galaxy M14 5G to Roku | Dr.fone</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/become-an-instagram-star-expert-5-strategies-and-illustrative-examples/"><u>Become an Instagram Star Expert 5 Strategies and Illustrative Examples</u></a></li>
<li><a href="https://win-great.techidaily.com/comprehensive-tutorial-on-vcenter-backups-and-restoration-processes/"><u>Comprehensive Tutorial on vCenter Backups & Restoration Processes</u></a></li>
<li><a href="https://win-great.techidaily.com/fonebackup-wie-sie-mp4-videos-effizient-auf-die-kamerarolle-ihres-iphone-sparen/"><u>FoneBackup: Wie Sie MP4 Videos Effizient Auf Die Kamerarolle Ihres iPhone Sparen</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/in-2024-how-to-change-your-sim-pin-code-on-your-honor-magic-5-phone-by-drfone-android/"><u>In 2024, How To Change Your SIM PIN Code on Your Honor Magic 5 Phone</u></a></li>
<li><a href="https://vimeo-videos.techidaily.com/in-2024-tactics-for-smoothly-importing-movies-to-vimeo-from-wmm/"><u>In 2024, Tactics for Smoothly Importing Movies to Vimeo From WMM</u></a></li>
<li><a href="https://win-great.techidaily.com/olympus-oder-sony-voice-recorders-methoden-zum-wiederherstellen-geloschter-aufnahmen/"><u>Olympus Oder Sony Voice Recorders: Methoden Zum Wiederherstellen Gelöschter Aufnahmen!</u></a></li>
<li><a href="https://techno-recovery.techidaily.com/ray-tracing-explained-the-key-to-photorealism-in-visual-media/"><u>Ray Tracing Explained: The Key to Photorealism in Visual Media</u></a></li>
<li><a href="https://win-great.techidaily.com/strategie-semplici-e-rapide-come-installare-windows-11-su-un-nuovo-pc/"><u>Strategie Semplici E Rapide: Come Installare Windows 11 Su Un Nuovo PC</u></a></li>
<li><a href="https://screen-video-capture.techidaily.com/transform-slideshow-into-video/"><u>Transform Slideshow Into Video</u></a></li>
<li><a href="https://win-great.techidaily.com/vom-alt-ins-neue-transition-von-active-directory-versionen-ad2008-auf-ad201-mit-optimaler-migrations-taktik/"><u>Vom Alt Ins Neue: Transition Von Active Directory Versionen (AD2008 Auf AD201#) Mit Optimaler Migrations-Taktik</u></a></li>
<li><a href="https://win-great.techidaily.com/windows-7usb/"><u>Windows 7におけるUSBフラッシュドライブのパスワード保護手順２点披露</u></a></li>
<li><a href="https://win-great.techidaily.com/effektivnye-metody-kopirovaniya-zagruzochnogo-diska-na-usb-obshij-process-i-rekomendacii/"><u>Эффективные Методы Копирования Загрузочного Диска На USB: Общий Процесс И Рекомендации</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/PD0vq5qAYkw?si=5H3KWtCfUOYg1Nlv&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

