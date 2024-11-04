---
title: Understanding Input Events Like onKeyPress and onClick Within EmEditor
date: 2024-11-02T19:42:35.114Z
updated: 2024-11-03T22:40:08.546Z
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
<li><a href="https://instagram-video-recordings.techidaily.com/new-2024-approved-avoiding-unauthorized-use-mastering-photowatermarking-on-instagram/"><u>[New] 2024 Approved Avoiding Unauthorized Use Mastering Photowatermarking on Instagram</u></a></li>
<li><a href="https://extra-skills.techidaily.com/2024-approved-spearheading-groundbre-folks-in-vr-space/"><u>2024 Approved Spearheading Groundbre Folks In VR Space</u></a></li>
<li><a href="https://win-great.techidaily.com/complete-guide-to-deleting-shared-images-from-iphone-and-ipad-ios-18-and-17/"><u>Complete Guide to Deleting Shared Images From iPhone and iPad (iOS 18 & 17)</u></a></li>
<li><a href="https://win-great.techidaily.com/complete-step-by-step-methods-for-retrieving-lost-documents-from-your-hard-drive-via-command-line-tools/"><u>Complete Step-by-Step Methods for Retrieving Lost Documents From Your Hard Drive via Command Line Tools</u></a></li>
<li><a href="https://win-great.techidaily.com/fehlerbehebung-fur-die-windows-11-datentragerbereinigungsfunktion-entdeckt-sie-7-effektive-losungen/"><u>Fehlerbehebung Für Die Windows 11-Datenträgerbereinigungsfunktion: Entdeckt Sie 7 Effektive Lösungen!</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/in-2024-hacks-to-do-pokemon-go-trainer-battles-for-itel-a70-drfone-by-drfone-virtual-android/"><u>In 2024, Hacks to do pokemon go trainer battles For Itel A70 | Dr.fone</u></a></li>
<li><a href="https://activate-lock.techidaily.com/in-2024-how-to-successfully-bypass-icloud-activation-lock-from-iphone-8-plus-by-drfone-ios/"><u>In 2024, How to Successfully Bypass iCloud Activation Lock from iPhone 8 Plus</u></a></li>
<li><a href="https://unlock-android.techidaily.com/in-2024-mastering-android-device-manager-the-ultimate-guide-to-unlocking-your-google-pixel-8-pro-device-by-drfone-android/"><u>In 2024, Mastering Android Device Manager The Ultimate Guide to Unlocking Your Google Pixel 8 Pro Device</u></a></li>
<li><a href="https://win-great.techidaily.com/norton-ghost-aomei-backupper/"><u>Norton Ghost 無料 同等品質：AOMEI Backupperスタンダード版</u></a></li>
<li><a href="https://win-great.techidaily.com/recover-deleted-photos-from-fujifilm-cameras-eine-schritt-fur-schritt-anleitung/"><u>Recover Deleted Photos From FujiFilm Cameras - Eine Schritt-Für-Schritt Anleitung</u></a></li>
<li><a href="https://screen-recording.techidaily.com/swiftclick-retrorecall-video-for-2024/"><u>SwiftClick RetroRecall Video for 2024</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2100530/7443" target="_top" id="2100530">
  <img src="//a.impactradius-go.com/display-ad/7443-2100530" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2100530/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

