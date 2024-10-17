---
title: Understanding Input Events Like onKeyPress and onClick Within EmEditor
date: 2024-10-16T16:03:46.457Z
updated: 2024-10-17T16:36:13.212Z
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
<li><a href="https://instagram-video-recordings.techidaily.com/new-posting-vimeo-video-masterclass-for-instagramers-for-2024/"><u>[New] Posting Vimeo Video Masterclass for Instagramers for 2024</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/updated-2024-approved-techniques-to-enhance-your-slow-motion-photos-for-instagram-audiences/"><u>[Updated] 2024 Approved Techniques to Enhance Your Slow Motion Photos for Instagram Audiences</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/updated-charting-your-course-through-youtube-compliance-for-2024/"><u>[Updated] Charting Your Course Through YouTube Compliance for 2024</u></a></li>
<li><a href="https://youtube-video-recordings.techidaily.com/updated-efficient-ad-elimination-select-7-android-adblockers/"><u>[Updated] Efficient Ad Elimination Select 7 Android AdBlockers</u></a></li>
<li><a href="https://article-tips.techidaily.com/updated-in-2024-refining-your-tiktok-profile-age-with-ease/"><u>[Updated] In 2024, Refining Your TikTok Profile Age with Ease</u></a></li>
<li><a href="https://facebook-videos.techidaily.com/updated-unearthing-your-favorites-facebook-watch-list-access-for-2024/"><u>[Updated] Unearthing Your Favorites Facebook Watch List Access for 2024</u></a></li>
<li><a href="https://win-great.techidaily.com/comment-reussir-une-copie-dynamique-dun-disque-dur-avec-le-meilleur-logiciel-de-clonage/"><u>Comment Réussir Une Copie Dynamique D'un Disque Dur Avec Le Meilleur Logiciel De Clonage ?</u></a></li>
<li><a href="https://win-great.techidaily.com/como-recuperar-archivos-de-un-disco-flash-ya-formateado-con-eficiencia/"><u>Cómo Recuperar Archivos De Un Disco Flash Ya Formateado Con Eficiencia</u></a></li>
<li><a href="https://win-great.techidaily.com/fixing-the-problem-of-non-authenticated-clients-in-vmware-management-services/"><u>Fixing the Problem of Non-Authenticated Clients in VMware Management Services</u></a></li>
<li><a href="https://android-transfer.techidaily.com/how-to-use-phone-clone-to-migrate-your-vivo-y100-data-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>How to Use Phone Clone to Migrate Your Vivo Y100 Data? | Dr.fone</u></a></li>
<li><a href="https://win-great.techidaily.com/mastering-clonezilla-backup-to-revive-a-specific-file-discover-the-top-3-techniques/"><u>Mastering Clonezilla Backup to Revive a Specific File: Discover the Top 3 Techniques</u></a></li>
<li><a href="https://win-great.techidaily.com/programmwiederherstellung-im-ordner-windowsold-auf-deinem-windows-11-pc-einfache-tipps-und-tricks/"><u>Programmwiederherstellung Im Ordner 'Windows.old' Auf Deinem Windows 11 PC: Einfache Tipps Und Tricks</u></a></li>
<li><a href="https://hardware-help.techidaily.com/step-by-step-how-to-easily-keep-your-lenovo-pc-drivers-current/"><u>Step-by-Step: How to Easily Keep Your Lenovo PC Drivers Current</u></a></li>
<li><a href="https://win-solutions.techidaily.com/troubleshooting-steps-for-successful-age-of-empires-iv-installation-on-ms-store/"><u>Troubleshooting Steps for Successful Age of Empires IV Installation on MS Store</u></a></li>
<li><a href="https://win-great.techidaily.com/windows0x81000203/"><u>トラブルシューティング成功： Windowsの復元エラー0x81000203を解決する方法</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2049369/7443" target="_top" id="2049369">
  <img src="//a.impactradius-go.com/display-ad/7443-2049369" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2049369/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

