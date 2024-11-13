---
title: Understanding Input Events Like onKeyPress and onClick Within EmEditor
date: 2024-11-11T00:05:46.072Z
updated: 2024-11-12T18:45:58.819Z
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
<li><a href="https://facebook-video-footage.techidaily.com/new-2024-approved-cracking-the-code-calculating-your-income-from-youtubes-cpm/"><u>[New] 2024 Approved Cracking the Code Calculating Your Income From YouTube's CPM</u></a></li>
<li><a href="https://fox-access.techidaily.com/new-iphones-prime-camera-utilities-for-2024/"><u>[New] IPhone's Prime Camera Utilities for 2024</u></a></li>
<li><a href="https://some-skills.techidaily.com/new-the-complete-guide-to-transforming-your-footages-hue/"><u>[New] The Complete Guide to Transforming Your Footage's Hue</u></a></li>
<li><a href="https://fox-friendly.techidaily.com/updated-in-2024-superior-methods-transforming-pinterest-visuals-into-audios/"><u>[Updated] In 2024, Superior Methods Transforming Pinterest Visuals Into Audios</u></a></li>
<li><a href="https://win-great.techidaily.com/1728493095708-usb/"><u>如何使用USB线从手机移动设备传送图片到个人电脑</u></a></li>
<li><a href="https://screen-capture.techidaily.com/chill-bites-analysis-in-depth-review-of-ice-cream-recorder/"><u>Chill Bites Analysis In-Depth Review of Ice Cream Recorder</u></a></li>
<li><a href="https://win-great.techidaily.com/comment-dejouez-les-plantages-reguliers-de-votre-systeme-dexploitation-windows-11-guide-pratique-en-6-etapes/"><u>Comment Déjouez Les Plantages Réguliers De Votre Système D'Exploitation Windows 11 : Guide Pratique en 6 Étapes</u></a></li>
<li><a href="https://win-great.techidaily.com/complete-tutorial-updating-your-vcenter-single-sign-on-sso-domain-and-resolving-frequent-problems/"><u>Complete Tutorial: Updating Your vCenter Single Sign-On (SSO) Domain & Resolving Frequent Problems</u></a></li>
<li><a href="https://win-great.techidaily.com/guida-passo-passo-allesecuzione-della-sincronizzazione-attiva-con-aomei-backupper/"><u>Guida Passo-Passo All'Esecuzione Della Sincronizzazione Attiva Con AOMEI Backupper</u></a></li>
<li><a href="https://win-great.techidaily.com/how-to-successfully-transfer-your-data-from-dell-hdd-to-ssd-in-windows-10-or-11-step-by-step-guide-for-a-functional-boot/"><u>How to Successfully Transfer Your Data From Dell HDD to SSD in Windows 10 or 11 - Step-by-Step Guide for a Functional Boot</u></a></li>
<li><a href="https://extra-skills.techidaily.com/in-2024-leading-action-cameras-for-thrill-seekers/"><u>In 2024, Leading Action Cameras for Thrill Seekers</u></a></li>
<li><a href="https://win-great.techidaily.com/strategie-ottimizzate-per-la-compressione-dei-dati-immagine-ed-efficiente-utilizzo-dello-spazio-del-disco-rigido/"><u>Strategie Ottimizzate per La Compressione Dei Dati Immagine Ed Efficiente Utilizzo Dello Spazio Del Disco Rigido</u></a></li>
<li><a href="https://data-safeguard.techidaily.com/website-efficiency-boosted-by-cookiebot-technology/"><u>Website Efficiency Boosted by Cookiebot Technology</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/what-is-the-best-pokemon-for-pokemon-pvp-ranking-on-zte-axon-40-lite-drfone-by-drfone-virtual-android/"><u>What is the best Pokemon for pokemon pvp ranking On ZTE Axon 40 Lite? | Dr.fone</u></a></li>
<li><a href="https://win-great.techidaily.com/windows-11-10-8-or-7-how-to-transfer-files-between-computers/"><u>Windows 11, 10, 8, or 7 - How to Transfer Files Between Computers</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2100527/7443" target="_top" id="2100527">
  <img src="//a.impactradius-go.com/display-ad/7443-2100527" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2100527/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

