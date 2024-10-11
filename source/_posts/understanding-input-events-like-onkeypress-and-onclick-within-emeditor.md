---
title: Understanding Input Events Like onKeyPress and onClick Within EmEditor
date: 2024-10-07T23:50:49.823Z
updated: 2024-10-11T02:19:23.891Z
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
<li><a href="https://win-great.techidaily.com/windows202/"><u>【おすすめ】Windowsで使える最新動画制作ツール202</u></a></li>
<li><a href="https://win-great.techidaily.com/1726030082324-windows-10/"><u>新規ユーザーのためのWindows 10動画圧縮手引き - シンプルな方法</u></a></li>
<li><a href="https://hardware-tips.techidaily.com/1723175652746-heavenly-computer-components-await-embrace-the-pleasant-surprise-of-flower-scented-thermal-paste/"><u>Heavenly Computer Components Await: Embrace the Pleasant Surprise of Flower-Scented Thermal Paste</u></a></li>
<li><a href="https://review-topics.techidaily.com/how-to-update-iphone-14-plus-without-losing-anything-drfone-by-drfone-ios-system-repair-ios-system-repair/"><u>How to Update iPhone 14 Plus without Losing Anything? | Dr.fone</u></a></li>
<li><a href="https://video-screen-grab.techidaily.com/in-2024-transform-meetings-with-easy-to-follow-zoom-sharing-tips/"><u>In 2024, Transform Meetings with Easy-to-Follow Zoom Sharing Tips</u></a></li>
<li><a href="https://fox-hovers.techidaily.com/perfecting-self-portraits-iphones-burst-capability-for-2024/"><u>Perfecting Self-Portraits IPhone's Burst Capability for 2024</u></a></li>
<li><a href="https://win-great.techidaily.com/quick-and-simple-guide-convert-your-mov-files-into-high-quality-webm-videos-in-just-5-steps/"><u>Quick & Simple Guide: Convert Your MOV Files Into High-Quality WebM Videos in Just 5 Steps</u></a></li>
<li><a href="https://tech-recovery.techidaily.com/revitalize-your-viewing-experience-the-ultimate-tried-and-true-strategies-for-blue-tint-on-tvs-ranked-1-8/"><u>Revitalize Your Viewing Experience: The Ultimate Tried-and-True Strategies for Blue Tint on TVs, Ranked #1-8</u></a></li>
<li><a href="https://fake-location.techidaily.com/spoofing-life360-how-to-do-it-on-xiaomi-13t-drfone-by-drfone-virtual-android/"><u>Spoofing Life360 How to Do it on Xiaomi 13T? | Dr.fone</u></a></li>
<li><a href="https://win-great.techidaily.com/step-by-step-tutorial-on-cloning-securely-locked-dvd-content/"><u>Step-by-Step Tutorial on Cloning Securely Locked DVD Content</u></a></li>
<li><a href="https://facebook.techidaily.com/1719149444954-streamline-social-syncing-integrate-facebook-storage-with-top-services/"><u>Streamline Social Syncing: Integrate Facebook Storage with Top Services</u></a></li>
<li><a href="https://win-great.techidaily.com/ultimate-tutorial-mov-file-modification-techniques-for-windows-11-users/"><u>Ultimate Tutorial: MOV File Modification Techniques for Windows 11 Users</u></a></li>
<li><a href="https://win-great.techidaily.com/44oi44oo44op44or6zplusz5aow6lui5oplusb5oml6acg44ks6zug57se44gx44gf44ks44kk44oj/"><u>モノラル音声転換手順を集約したガイド</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2037319/7443" target="_top" id="2037319">
  <img src="//a.impactradius-go.com/display-ad/7443-2037319" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2037319/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

