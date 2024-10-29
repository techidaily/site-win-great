---
title: Overcoming Issues with New Line Character Recognition in the emEditor Text Editor
date: 2024-10-24T21:22:11.947Z
updated: 2024-10-29T04:37:40.709Z
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
<li><a href="https://graphic-issues.techidaily.com/triumph-mhw-error-12-dispatched-graphics-restored/"><u>[Triumph] MHW Error 12 Dispatched, Graphics Restored</u></a></li>
<li><a href="https://youtube-tips.techidaily.com/ed-in-2024-chart-toppers-unveiled-top-youtube-stars-and-their-subs/"><u>[Updated] In 2024, Chart-Toppers Unveiled Top YouTube Stars and Their Subs</u></a></li>
<li><a href="https://howto.techidaily.com/9-solutions-to-fix-process-system-isnt-responding-error-on-xiaomi-civi-3-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>9 Solutions to Fix Process System Isnt Responding Error on Xiaomi Civi 3 | Dr.fone</u></a></li>
<li><a href="https://data-wizards.techidaily.com/accessible-tech-stellar-enhances-data-recovery-simplicity/"><u>Accessible Tech: Stellar Enhances Data Recovery Simplicity</u></a></li>
<li><a href="https://win-great.techidaily.com/aomei-cloud-datenretentionspolitik-uberblick-und-anwendung/"><u>AOMEI Cloud Datenretentionspolitik: Überblick Und Anwendung</u></a></li>
<li><a href="https://screen-sharing-recording.techidaily.com/best-virtual-race-titles-reviewed/"><u>Best Virtual Race Titles Reviewed</u></a></li>
<li><a href="https://win-great.techidaily.com/comment-cloner-avec-excellence-vos-ssds-m2-nvme-les-deux-meilleures-methodes-a-privilegier-en-2024/"><u>Comment Cloner Avec Excellence Vos SSDs M.2 NVMe: Les Deux Meilleures Méthodes À Privilégier en 2024</u></a></li>
<li><a href="https://win-great.techidaily.com/common-challenges-during-the-setup-of-emeditor-text-editor-v7/"><u>Common Challenges During the Setup of EmEditor Text Editor V.7</u></a></li>
<li><a href="https://fox-boxes.techidaily.com/comprehensive-manual-on-morphvox-sound-alteration/"><u>Comprehensive Manual on MorphVOX Sound Alteration</u></a></li>
<li><a href="https://fake-location.techidaily.com/how-to-change-google-play-location-on-poco-c55-drfone-by-drfone-virtual-android/"><u>How to Change Google Play Location On Poco C55 | Dr.fone</u></a></li>
<li><a href="https://win-great.techidaily.com/how-to-securely-backup-your-windows-11-laptop-best-practices-and-tips/"><u>How to Securely Backup Your Windows 11 Laptop – Best Practices and Tips</u></a></li>
<li><a href="https://win-forum.techidaily.com/navigating-the-digital-sphere-with-leading-platforms-facebook-twitter-instagram-and-youtube-guides/"><u>Navigating the Digital Sphere with Leading Platforms: Facebook, Twitter, Instagram & Youtube Guides</u></a></li>
<li><a href="https://win-great.techidaily.com/strategies-efficaces-de-gestion-de-lespace-disque-pour-les-sauvegardes-aomei-comprendre-le-plan/"><u>Stratégies Efficaces De Gestion De L’Espace Disque Pour Les Sauvegardes AOMEI : Comprendre Le Plan</u></a></li>
<li><a href="https://some-guidance.techidaily.com/syncing-sounds-to-visuals-online-for-2024/"><u>Syncing Sounds to Visuals Online for 2024</u></a></li>
<li><a href="https://win-great.techidaily.com/troubleshooting-the-lenovo-bsod-simple-and-secure-solutions-to-resolve-error-code-0xc000021a/"><u>Troubleshooting the Lenovo BSOD: Simple & Secure Solutions to Resolve Error Code 0XC000021A</u></a></li>
<li><a href="https://ai-video-tools.techidaily.com/updated-transform-your-gopro-clips-a-step-by-step-mac-video-editing-guide-for-2024/"><u>Updated Transform Your GoPro Clips A Step-by-Step Mac Video Editing Guide for 2024</u></a></li>
<li><a href="https://win-great.techidaily.com/warum-machen-deine-speichermedien-gerausche-und-starten-nicht-sofortige-losungen/"><u>Warum Machen Deine Speichermedien Geräusche Und Starten Nicht? Sofortige Lösungen!</u></a></li>
<li><a href="https://win-great.techidaily.com/1728490076278-windows-10/"><u>Windows 10 誤始動ドライブのトラブルシューティング - パソコン問題の一環として</u></a></li>
<li><a href="https://win-great.techidaily.com/1728498324218-sd/"><u>ビデオ撮影用カメラから消えたSDカード情報を確実に取り戻せる方法</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135399/19272" target="_top" id="2135399">
  <img src="//a.impactradius-go.com/display-ad/19272-2135399" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135399/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

