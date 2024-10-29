---
title: Understanding Input Events Like onKeyPress and onClick Within EmEditor
date: 2024-10-23T00:45:03.027Z
updated: 2024-10-28T17:22:56.722Z
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
<li><a href="https://facebook-video-footage.techidaily.com/new-discovering-and-developing-your-personalized-mukbang-style-for-2024/"><u>[New] Discovering and Developing Your Personalized Mukbang Style for 2024</u></a></li>
<li><a href="https://win-great.techidaily.com/abgesicherter-betriebsmodus-fur-ihre-lenovo-maschine-mit-windows-11-komplette-anleitung-und-tipps/"><u>Abgesicherter Betriebsmodus Für Ihre Lenovo-Maschine Mit Windows 11 - Komplette Anleitung Und Tipps</u></a></li>
<li><a href="https://win-great.techidaily.com/comprehensive-step-by-step-tutorial-on-complete-iphone-data-backup-and-restoration/"><u>Comprehensive Step-by-Step Tutorial on Complete iPhone Data Backup & Restoration</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/does-edgeplus-2023-support-avchd-video-by-aiseesoft-video-converter-play-mts-on-android/"><u>Does Edge+ (2023) support AVCHD video?</u></a></li>
<li><a href="https://blog-min.techidaily.com/easy-conversion-techniques-from-avi-video-to-vob-playback-compatibility/"><u>Easy Conversion Techniques From AVI Video to VOB Playback Compatibility</u></a></li>
<li><a href="https://youtube-blog.techidaily.com/ating-the-financial-giants-mr-beast/"><u>Evaluating the Financial Giants Mr. Beast</u></a></li>
<li><a href="https://ios-unlock.techidaily.com/how-can-i-unlock-my-iphone-6-after-forgetting-my-pin-code-by-drfone-ios/"><u>How Can I Unlock My iPhone 6 After Forgetting my PIN Code?</u></a></li>
<li><a href="https://buynow-reviews.techidaily.com/improving-your-spotify-experience-by-protecting-recommendations-from-playlist-influence/"><u>Improving Your Spotify Experience by Protecting Recommendations From Playlist Influence</u></a></li>
<li><a href="https://win-great.techidaily.com/losungen-zur-wiederherstellung-von-defekten-transcend-sd-speicherkarten-ein-umfassender-leitfaden/"><u>Lösungen Zur Wiederherstellung Von Defekten Transcend SD-Speicherkarten: Ein Umfassender Leitfaden</u></a></li>
<li><a href="https://tech-revival.techidaily.com/navigate-with-ease-advanced-menu-options-for-linkedin-facebook-and-youtube-integration/"><u>Navigate with Ease: Advanced Menu Options for LinkedIn, Facebook & YouTube Integration</u></a></li>
<li><a href="https://win-great.techidaily.com/recuperacion-desde-una-restauracion-del-sistema-en-windows-11-explicada-tecnicas-efectivas-y-cuatro-soluciones-utiles/"><u>Recuperación Desde Una Restauración Del Sistema en Windows 11 Explicada: Técnicas Efectivas Y Cuatro Soluciones Útiles</u></a></li>
<li><a href="https://win-great.techidaily.com/tout-ce-quil-vous-faut-savoir-pour-cloner-votre-disque-dur-sur-un-ssd-en-seulement-3-etapes-simples/"><u>Tout Ce Qu'il Vous Faut Savoir Pour Cloner Votre Disque Dur Sur Un SSD en Seulement 3 Étapes Simples</u></a></li>
<li><a href="https://win-great.techidaily.com/transferieren-von-iphones-messaging-history-an-android-zwei-effektive-strategien-erklart/"><u>Transferieren Von iPhones Messaging History an Android - Zwei Effektive Strategien Erklärt!</u></a></li>
<li><a href="https://win-great.techidaily.com/1728490855390-windowsssd/"><u>Windowsで使いやすい完全無料のトップSSD移行ソフトウェア</u></a></li>
<li><a href="https://extra-tips.techidaily.com/x1000-video-world-comprehensive-sony-examination/"><u>X1000 Video World Comprehensive Sony Examination</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://dhgate.sjv.io/c/5597632/2106658/12108" target="_top" id="2106658">
  <img src="//a.impactradius-go.com/display-ad/12108-2106658" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://dhgate.sjv.io/i/5597632/2106658/12108" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

