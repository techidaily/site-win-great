---
title: Understanding Input Events Like onKeyPress and onClick Within EmEditor
date: 2024-11-17T16:51:34.640Z
updated: 2024-11-22T18:52:16.873Z
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
<li><a href="https://fox-links.techidaily.com/new-essentials-of-choosing-top-5-web-based-title-innovators/"><u>[New] Essentials of Choosing Top 5 Web-Based Title Innovators</u></a></li>
<li><a href="https://fox-info.techidaily.com/new-radiant-hue-tuner-program-for-2024/"><u>[New] Radiant Hue Tuner Program for 2024</u></a></li>
<li><a href="https://screen-recording.techidaily.com/updated-in-2024-ultimate-guide-to-iphone-7-screen-recording/"><u>[Updated] In 2024, Ultimate Guide to iPhone 7 Screen Recording</u></a></li>
<li><a href="https://win-great.techidaily.com/effective-methods-for-retrieving-lost-inx-file-data/"><u>Effective Methods for Retrieving Lost INX File Data</u></a></li>
<li><a href="https://article-files.techidaily.com/explore-the-premier-3d-blu-ray-systems-of-today/"><u>Explore The Premier 3D Blu-Ray Systems of Today</u></a></li>
<li><a href="https://win-great.techidaily.com/guide-complet-comment-effectuer-une-sauvegarde-de-son-nas-vers-un-hdd-extern/"><u>Guide Complet - Comment Effectuer Une Sauvegarde De Son NAS Vers Un HDD Extern</u></a></li>
<li><a href="https://win-great.techidaily.com/guide-de-copie-simple-dun-hdd-avec-windows-11-explications-claires-et-faciles/"><u>Guide De Copie Simple D'un HDD Avec Windows 11 - Explications Claires Et Faciles!</u></a></li>
<li><a href="https://win-great.techidaily.com/how-to-seamlessly-back-up-and-synchronize-your-external-hard-drives-using-google-drive/"><u>How to Seamlessly Back Up & Synchronize Your External Hard Drives Using Google Drive</u></a></li>
<li><a href="https://article-knowledge.techidaily.com/in-2024-in-depth-insight-into-final-cut-pro-editing/"><u>In 2024, In-Depth Insight Into Final Cut Pro Editing</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/in-2024-top-10-fingerprint-lock-apps-to-lock-your-nubia-phone-by-drfone-android/"><u>In 2024, Top 10 Fingerprint Lock Apps to Lock Your Nubia Phone</u></a></li>
<li><a href="https://win-great.techidaily.com/panduan-bantu-untuk-mengaweti-masalah-tabel-partisi-yang-putus-adaptive-memory-technology-windows/"><u>Panduan Bantu Untuk Mengaweti Masalah Tabel Partisi Yang Putus Adaptive Memory Technology (Windows)</u></a></li>
<li><a href="https://hardware-updates.techidaily.com/1722971856975-quick-and-simple-installation-of-ft232r-usb-uart-drivers-get-started-now/"><u>Quick and Simple Installation of FT232R USB UART Drivers - Get Started Now!</u></a></li>
<li><a href="https://media-tips.techidaily.com/reviving-disneyplus-success-top-6-essential-enhancements-for-growth/"><u>Reviving Disney+ Success: Top 6 Essential Enhancements for Growth</u></a></li>
<li><a href="https://win-webster.techidaily.com/unexpected-changes-in-emeditor-a-comprehensive-update-overview/"><u>Unexpected Changes in EmEditor: A Comprehensive Update Overview</u></a></li>
<li><a href="https://win-great.techidaily.com/windows-11-10-8-and-7-ultimate-guide-to-backing-up-hdd-before-formatting/"><u>Windows 11, 10, 8, and 7: Ultimate Guide to Backing Up HDD Before Formatting</u></a></li>
<li><a href="https://win-great.techidaily.com/windows-11-hdd/"><u>Windows 11用で人気のベスト HDD コピープログラム - 無料</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/E1ax-vnGdeo?si=bgTkOhOEwDTlRQE3&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

