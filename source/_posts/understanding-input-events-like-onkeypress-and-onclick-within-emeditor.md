---
title: Understanding Input Events Like onKeyPress and onClick Within EmEditor
date: 2024-11-29T18:00:10.112Z
updated: 2024-12-01T06:22:33.935Z
tags:
  - product
categories:
  - emeditor
thumbnail: https://thmb.techidaily.com/b478b0983a67f36010d885714312f70db32d5d3a2179d68b62f5c8d46f0ea38e.jpg
---

## Understanding Input Events Like onKeyPress and onClick Within EmEditor

November 23, 2008 at 5:12 pm [#6656](https://tools.techidaily.com/emeditor/products/) 

[![](https://secure.gravatar.com/avatar/d73fc2c7bd494149d303a2b87aa5a6d5?s=80&d=identicon&r=g)dreftymac](https://www.emeditor.com/forums/users/dreftymac/ "View dreftymac's profile")

Participant

I don’t know if there is a way to trigger a macro with a mouse click, but you can trigger a macro using a keyboard shortcut. You can also use a single keyboard shortcut to trigger multiple choices for the user, so you do not have to restrict your macro to doing just one “action”.

 The following example uses the document.selection and the CreatePopupMenu function inside a jsee macro. The popup menu gives the user multiple choices before displaying the result.
  

	var vtext   =   document.selection.Text;  

	var result  =   '';  

	var menu    =   CreatePopupMenu();              

	menu.Add("look north", 1);  

	menu.Add("look south", 2);  

	menu.Add("look east", 3);  

	result = menu.Track(0);              

	if(result != 0) {  

	    result  = (menu.GetText(result));  

	Window.alert([result,vtext].join(' '));

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
<li><a href="https://youtube-docs.techidaily.com/ajis-wealth-kid-star-earnings-surpass-major-celebrities/"><u>[New] Kaji’s Wealth Kid Star Earnings Surpass Major Celebrities</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/updated-in-2024-integrating-facebook-video-into-home-screen-apps/"><u>[Updated] In 2024, Integrating Facebook Video Into Home Screen Apps</u></a></li>
<li><a href="https://some-skills.techidaily.com/updated-the-ultimate-list-of-10-vectors-stock-pics-websites/"><u>[Updated] The Ultimate List of 10 Vectors Stock Pics Websites</u></a></li>
<li><a href="https://youtube-webster.techidaily.com/approved-empowered-by-numbers-decoding-youtube-analytics/"><u>2024 Approved Empowered by Numbers Decoding YouTube Analytics</u></a></li>
<li><a href="https://location-fake.techidaily.com/a-detailed-vpna-fake-gps-location-free-review-on-nokia-c02-drfone-by-drfone-virtual-android/"><u>A Detailed VPNa Fake GPS Location Free Review On Nokia C02 | Dr.fone</u></a></li>
<li><a href="https://win-great.techidaily.com/como-recuperar-mundos-de-minecraft-borrados-en-windows-y-dispositivos-moviles/"><u>Cómo Recuperar Mundos De Minecraft Borrados en Windows Y Dispositivos Móviles</u></a></li>
<li><a href="https://win-great.techidaily.com/complete-troubleshooting-guide-for-resolving-windows-8-error-code-0x8024000b/"><u>Complete Troubleshooting Guide for Resolving Windows 8 Error Code 0X8024000B</u></a></li>
<li><a href="https://win-great.techidaily.com/grande-disco-guida-completa-alla-clonazione-disco-con-clonezilla-soluzioni-di-backup-e-ripristino/"><u>Grande Disco: Guida Completa Alla Clonazione Disco Con Clonezilla - Soluzioni Di Backup E Ripristino</u></a></li>
<li><a href="https://android-transfer.techidaily.com/in-2024-how-to-transfer-music-from-honor-magic-6-to-ipod-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>In 2024, How to Transfer Music from Honor Magic 6 to iPod | Dr.fone</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/in-2024-preparation-to-beat-giovani-in-pokemon-go-for-infinix-hot-40-pro-drfone-by-drfone-virtual-android/"><u>In 2024, Preparation to Beat Giovani in Pokemon Go For Infinix Hot 40 Pro | Dr.fone</u></a></li>
<li><a href="https://win-great.techidaily.com/macaomei-backupper/"><u>Mac电脑中通过AOMEI Backupper实现简单数据备份方法</u></a></li>
<li><a href="https://win-great.techidaily.com/schritt-fur-schritt-anleitung-wie-fugt-man-externe-videodateien-auf-ihr-iphone-importieren/"><u>Schritt-Für-Schritt-Anleitung: Wie Fügt Man Externe Videodateien Auf Ihr iPhone Importieren</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/the-ultimate-list-of-powerful-pc-screencasters-for-2024/"><u>The Ultimate List of Powerful PC Screencasters for 2024</u></a></li>
<li><a href="https://win-great.techidaily.com/unlocking-seamless-two-way-communication-resolving-single-direction-issues-with-iphone-and-mac-airdrop/"><u>Unlocking Seamless Two-Way Communication: Resolving Single Direction Issues with iPhone & Mac AirDrop</u></a></li>
<li><a href="https://win-great.techidaily.com/1728508232125-windows-1011-hdd/"><u>Windows 10/11用ディスク容量解放: HDDの初期設定と完全な消去方法</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/JMgRzDANfSQ?si=NDy01ntXGGOi1Uxs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

