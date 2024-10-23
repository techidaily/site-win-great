---
title: Understanding Input Events Like onKeyPress and onClick Within EmEditor
date: 2024-10-19T22:29:42.658Z
updated: 2024-10-22T22:26:34.088Z
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
<li><a href="https://fox-links.techidaily.com/new-helmet-hats-a-comprehensive-look-at-best-cams-in-bike-culture-for-2024/"><u>[New] Helmet Hats A Comprehensive Look at Best Cams in Bike Culture for 2024</u></a></li>
<li><a href="https://extra-lessons.techidaily.com/2024-approved-10-commandments-of-eye-catching-podcast-album-imagery/"><u>2024 Approved 10 Commandments of Eye-Catching Podcast Album Imagery</u></a></li>
<li><a href="https://buynow-marvelous.techidaily.com/analyzing-the-motorola-edgeplus-a-bargain-compromise-on-luxury-standards/"><u>Analyzing the Motorola Edge+: A Bargain Compromise on Luxury Standards</u></a></li>
<li><a href="https://win-great.techidaily.com/como-habilitar-la-transferencia-automatica-de-archivos-entre-carpetas-locales-y-su-nas-synology-mediante-windows/"><u>Cómo Habilitar La Transferencia Automática De Archivos Entre Carpetas Locales Y Su NAS Synology Mediante Windows</u></a></li>
<li><a href="https://win-great.techidaily.com/effizientes-wiederherstellen-von-bildern-aus-dem-papierkorb-3-kostenlose-methoden/"><u>Effizientes Wiederherstellen Von Bildern Aus Dem Papierkorb – 3 Kostenlose Methoden</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/innovative-iphone-tactics-for-capturing-glass-surfaces-for-2024/"><u>Innovative iPhone Tactics for Capturing Glass Surfaces for 2024</u></a></li>
<li><a href="https://win-great.techidaily.com/la-aplicacion-mas-eficaz-para-la-migracion-de-datos-en-samsung-compatible-con-windows-7-8-10-y-11/"><u>La Aplicación Más Eficaz Para La Migración De Datos en Samsung: Compatible Con Windows 7, 8, 10 Y 11</u></a></li>
<li><a href="https://win-tutorials.techidaily.com/online-gratuit-konverteren-van-wma-naar-flv-movavi-streaming-solutions/"><u>Online Gratuit Konverteren Van WMA Naar FLV - Movavi Streaming Solutions</u></a></li>
<li><a href="https://win-great.techidaily.com/problemas-para-acceder-a-archivos-inactivos-durante-la-sincronizacion-en-sistemas-operativos-windows-11/"><u>Problemas Para Acceder a Archivos Inactivos Durante La Sincronización en Sistemas Operativos Windows 11</u></a></li>
<li><a href="https://techidaily.com/sign-word-online-add-signature-to-word-for-free-by-ldigisigner-sign-a-word-sign-a-word/"><u>Sign Word Online - Add Signature to Word for Free</u></a></li>
<li><a href="https://win-great.techidaily.com/understanding-differences-what-sets-deleting-files-apart-from-uninstalling-programs/"><u>Understanding Differences: What Sets Deleting Files Apart From Uninstalling Programs</u></a></li>
<li><a href="https://youtube-blog.techidaily.com/-journey-discovering-top-online-practitioners-for-2024/"><u>Yogic Journey Discovering Top Online Practitioners for 2024</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2082521/7443" target="_top" id="2082521">
  <img src="//a.impactradius-go.com/display-ad/7443-2082521" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2082521/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

