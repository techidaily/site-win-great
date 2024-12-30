---
title: Understanding Input Events Like onKeyPress and onClick Within EmEditor
date: 2024-12-26T17:59:58.464Z
updated: 2024-12-29T19:05:44.678Z
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
<li><a href="https://youtube-docs.techidaily.com/ed-in-2024-double-delight-endless-looping-of-youtube-videos-for-tvs/"><u>[Updated] In 2024, Double Delight Endless Looping of YouTube Videos for TVs</u></a></li>
<li><a href="https://youtube-tips.techidaily.com/ed-in-2024-windows-movie-maker-a-toolkit-for-youtube-videographers/"><u>[Updated] In 2024, Windows Movie Maker A Toolkit for YouTube Videographers</u></a></li>
<li><a href="https://win-great.techidaily.com/decoding-crypto-trends-expert-techniques-for-interpreting-candlestick-charts-using-yl-solutions/"><u>Decoding Crypto Trends: Expert Techniques for Interpreting Candlestick Charts Using YL Solutions</u></a></li>
<li><a href="https://buynow-help.techidaily.com/ensuring-regularity-in-eating-habits-introducing-the-petsafe-auto-feeder-six-serve-model/"><u>Ensuring Regularity in Eating Habits - Introducing the PetSafe Auto-Feeder Six Serve Model</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/in-2024-the-best-8-vpn-hardware-devices-reviewed-on-honor-magic-6-drfone-by-drfone-virtual-android/"><u>In 2024, The Best 8 VPN Hardware Devices Reviewed On Honor Magic 6 | Dr.fone</u></a></li>
<li><a href="https://facebook.techidaily.com/1719149540102-personalize-your-playlists-anywhere-fbs-mini-panel-feature-spotify/"><u>Personalize Your Playlists Anywhere - FB's Mini-Panel Feature, Spotify!</u></a></li>
<li><a href="https://win-great.techidaily.com/recover-deleted-or-corrupted-windows-system-files-with-ease-expert-advice-from-yl-software/"><u>Recover Deleted or Corrupted Windows System Files with Ease - Expert Advice From YL Software</u></a></li>
<li><a href="https://win-great.techidaily.com/sing-your-heart-out-with-the-latest-additions-to-our-karaoke-library-special-early-access-for-subscribers-of-karaoke-cloud-pro/"><u>Sing Your Heart Out with the Latest Additions to Our Karaoke Library - Special Early Access for Subscribers of Karaoke Cloud Pro!</u></a></li>
<li><a href="https://win-great.techidaily.com/step-by-step-tutorial-on-utilizing-windows-defender-for-enhanced-security-yl-software-insights/"><u>Step-by-Step Tutorial on Utilizing Windows Defender for Enhanced Security - YL Software Insights</u></a></li>
<li><a href="https://on-screen-recording.techidaily.com/strategies-for-syncing-zoom-meetings-across-devices/"><u>Strategies for Syncing Zoom Meetings Across Devices</u></a></li>
<li><a href="https://win-great.techidaily.com/try-the-latest-karaoke-pro-software-free-demo-of-karaoki-v097978-by-pioneer-dj/"><u>Try the Latest Karaoke Pro Software - Free Demo of Karaoki v0.9.7978 by Pioneer DJ</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/_O8m9KphYzs?si=jITthzeyX_Kmt9X2" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

