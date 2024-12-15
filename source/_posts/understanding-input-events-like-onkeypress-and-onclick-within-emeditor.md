---
title: Understanding Input Events Like onKeyPress and onClick Within EmEditor
date: 2024-12-07T16:08:47.836Z
updated: 2024-12-14T16:00:57.415Z
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
<li><a href="https://facebook-clips.techidaily.com/new-2023-how-to-autoplay-facebook-videos-for-2024/"><u>[New] 2023 | How to Autoplay Facebook Videos for 2024</u></a></li>
<li><a href="https://some-approaches.techidaily.com/updated-unveiling-windows-media-seamless-cd-extraction/"><u>[Updated] Unveiling Windows Media Seamless CD Extraction</u></a></li>
<li><a href="https://some-approaches.techidaily.com/2024-approved-top-20-unlimited-cloud-storage-solutions-up-to-1tb/"><u>2024 Approved Top 20 Unlimited Cloud Storage Solutions, Up To 1TB</u></a></li>
<li><a href="https://win11-tips.techidaily.com/bypassing-the-obstacle-dealing-with-device-error-22-on-windows-11/"><u>Bypassing the Obstacle: Dealing with Device Error 22 on Windows 11</u></a></li>
<li><a href="https://win-great.techidaily.com/check-if-your-graphics-card-works-with-windows-a-comprehensive-guide-by-yl-computing/"><u>Check If Your Graphics Card Works With Windows: A Comprehensive Guide by YL Computing</u></a></li>
<li><a href="https://win-great.techidaily.com/connect-your-pc-to-the-web-a-simple-guide-from-yl-computing-essential-steps-explained/"><u>Connect Your PC to the Web: A Simple Guide From YL Computing - Essential Steps Explained</u></a></li>
<li><a href="https://win-great.techidaily.com/get-started-with-mining-pools-a-comprehensive-guide-by-yl-computing/"><u>Get Started with Mining Pools: A Comprehensive Guide by YL Computing</u></a></li>
<li><a href="https://facebook.techidaily.com/premium-metas-gain-verified-identity-badge/"><u>Premium Metas: Gain Verified Identity Badge</u></a></li>
<li><a href="https://win-great.techidaily.com/solving-the-issue-why-wont-your-pc-detect-the-graphics-card-expert-advice-by-yl-computing/"><u>Solving the Issue: Why Won't Your PC Detect the Graphics Card? Expert Advice by YL Computing</u></a></li>
<li><a href="https://win-great.techidaily.com/unlocking-faster-performance-a-step-by-step-guide-to-activating-hardware-acceleration-in-windows-tips-from-yl-computing/"><u>Unlocking Faster Performance: A Step-by-Step Guide to Activating Hardware Acceleration in Windows - Tips From YL Computing</u></a></li>
<li><a href="https://games-able.techidaily.com/your-companion-list-greatest-mobile-mmos/"><u>Your Companion List: Greatest Mobile MMOs</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/Wy0uYNNdMDM?si=5ir7EHlr0CkpcYOT" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

