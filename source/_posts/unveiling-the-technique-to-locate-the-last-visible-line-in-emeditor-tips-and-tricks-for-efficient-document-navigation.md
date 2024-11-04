---
title: "Unveiling the Technique to Locate the Last Visible Line in EmEditor: Tips and Tricks for Efficient Document Navigation"
date: 2024-11-02T19:49:49.781Z
updated: 2024-11-03T16:09:30.031Z
tags:
  - product
categories:
  - emeditor
thumbnail: https://thmb.techidaily.com/57a65c2b181c750fb6364283d0997e4f78e21ce130fdd9928a29e2fa7b69ddd1.jpg
---

## Unveiling the Technique to Locate the Last Visible Line in EmEditor: Tips and Tricks for Efficient Document Navigation

Tagged: [filter](https://tools.techidaily.com/emeditor/products/), [last visible line](https://tools.techidaily.com/emeditor/products/), [line number](https://tools.techidaily.com/emeditor/products/), [macro](https://tools.techidaily.com/emeditor/products/)

Viewing 9 posts - 1 through 9 (of 9 total)

* Author  
Posts
* August 30, 2016 at 3:51 pm [#21031](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/21bf85a5da27278c7f73ff85a8eb81ab?s=80&d=identicon&r=g)LifeTimer](https://www.emeditor.com/forums/users/lifetimer/ "View LifeTimer's profile")  
Participant  
I’m using a macro (in Cell Selection Mode) to select all the data in the column where the “cell cursor” is currently at. It looks like this:  
```  
	document.selection.SetActivePoint(eePosCell, document.selection.GetActivePointX(eePosCell), 2, false);  
	document.selection.SetActivePoint(eePosCell, document.selection.GetActivePointX(eePosCell), document.GetLines() - 1, true);  
```  
It works great when there is no active filter, but as soon as any line at the end of the file is currently filtered-out, it won’t work. It will then instead select all the columns including **_and to the left of_** the column where the “cell cursor” is currently at.  
The simple explanation for this is that the expression “document.GetLines() – 1” will not move the cursor from the last (empty) line above it in the filtered data (because the line number of that line will still be less than “document.GetLines() – 1” if any lines have been filtered-out inbetween the end of the document and the last **_visible_** (= non-filtered out) line in the document). Thus, the cell cursor will “snap left” on the very last line of the file (which is always empty, therefore bringing the cell cursor all the way to the left, consequently selecting also all the columns to the left of the intended column).  
So, my question is therefore: Is there any way to get the line numbers of only the **_visible_** lines (i.e. those that are not hidden by the filter) in a file, from a macro?  
If not, how can I go about selecting the entire contents of a single column from a macro in the above described scenario?  
Example data (with example line numbers to the left):  
```  
1: col1;col2;col3  
2: 1;2;3  
3: 11;22;33  
4: 111;222;333  
10:  
```  
In this case, lines 5-9 of the file have been filtered-out by a filter expression, therefore not being visible in the editor window.  
So, what I want in this example is to get the number of the last visible line (i.e. nr 4, which is the last visible line before the very last line which in this case is nr 10, where the last one is always empty without any cells, except the “artificial” cell being placed to the very left), or any other method to reliably select the entire data contents (i.e. rows 2-4) of this column.  
Are any of these two things currently possible from EmEditor macros, or could you otherwise possibly add the possibility to do any of these two things?  
September 6, 2016 at 11:30 pm [#21032](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/a0a6377144ed3636f985d87303f65ed2?s=80&d=identicon&r=g)Yutaka Emura](https://www.emeditor.com/forums/users/yemura/ "View Yutaka Emura's profile")  
Keymaster  
Hello LifeTimer,  
The following macro should get the number of visible lines.  
`n = document.GetLines(eeGetLineView);`  
Can you please try and let me know if you have further questions?  
September 21, 2016 at 6:41 am [#21073](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/21bf85a5da27278c7f73ff85a8eb81ab?s=80&d=identicon&r=g)LifeTimer](https://www.emeditor.com/forums/users/lifetimer/ "View LifeTimer's profile")  
Participant  
Thanks for your reply!  
Unfortunately, this is not a solution for the problem. :-(
Even though it works when **_only_** rows at the very end of the file has been filtered away, it does not work if any other rows higher up in the document has been filtered away also.  
Example:  
Unfiltered document contents:  
```  
col1,col2,col3  
1,2,3  
aaa,bbb,ccc  
aaa,bbb,ccc  
11,22,33  
111,222,333  
xxx,yyy,zzz  
xxx,yyy,zzz  
xxx,yyy,zzz  
xxx,yyy,zzz  
xxx,yyy,zzz  
```  
After filtering the last rows (e.g. filtering away “xxx”):  
```  
col1,col2,col3  
1,2,3  
aaa,bbb,ccc  
aaa,bbb,ccc  
11,22,33  
111,222,333  
```  
As mentioned above, the selection macro in my first post (modified with your suggestion of the _eeGetLineView_ parameter to the _document.GetLines()_ method) does indeed work now, BUT, if we also filter away some other lines, e.g. the ones containing “aaa”, we get the following visible document contents:  
```  
col1,col2,col3  
1,2,3  
11,22,33  
111,222,333  
```  
And if we then try to run the macro, the selection is cut short and does not cover the full column (the last line is not selected, and the more lines we filter away, the more lines will not be selected at the bottom).  
The problem is apparently that the _SetActivePoint()_ method uses absolute line numbers (i.e. ignoring that rows have been filtered away), while the _document.GetLines()_ method always returns a total _count_ of lines (visible or not). So we would either need the _SetActivePoint()_ method to also be able to use relative line numbers (i.e. after filtering), or need some completely other method to return the absolute line number of the last visible (non empty) line (for example named “document.GetLastVisibleLineNumber()”), in order to be able to perform this simple operation of selecting the contents of a column?  
Here is the full macro code, modified with your suggested _eeGetLineView_ parameter, for reference:  
```  
document.selection.SetActivePoint(eePosCell, document.selection.GetActivePointX(eePosCell), 2, false);  
document.selection.SetActivePoint(eePosCell, document.selection.GetActivePointX(eePosCell), document.GetLines(eeGetLineView) - 1, true);  
```  
September 26, 2016 at 1:07 pm [#21081](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/a0a6377144ed3636f985d87303f65ed2?s=80&d=identicon&r=g)Yutaka Emura](https://www.emeditor.com/forums/users/yemura/ "View Yutaka Emura's profile")  
Keymaster  
Hello,  
`document.GetLines(eeGetLineView);`  
should always return the number of only visible lines. Please make sure you add the “eeGetLinesView” flag as written above.  
Can you make sure you use the latest version of EmEditor?  
If the problem persists, please write the issue with a very simple example with a few sentences (as simple as possible).  
Thank you,  
September 26, 2016 at 2:20 pm [#21082](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/21bf85a5da27278c7f73ff85a8eb81ab?s=80&d=identicon&r=g)LifeTimer](https://www.emeditor.com/forums/users/lifetimer/ "View LifeTimer's profile")  
Participant  
Sorry if I was unclear. Yes, the _eeGetLineView_ parameter to the _document.GetLines()_ method does indeed return the number of visible lines. Unfortunately this is not the problem though.  
The problem is that when I then want to use this number to move the cell cursor in the filtered document data, it turns out that the _document.selection.SetActivePoint()_ method only uses **absolute line numbers** (i.e. the line numbers that are listed to the left in EmEditor, contrary to the target line’s number in the order of visible lines from the top of the document), and these absolute line numbers do not change when filtering the data, which in turn means that the result returned from _document.GetLines(eeGetLineView)_ is sadly of no use at all for knowing how to make _document.selection.SetActivePoint()_ position the cell cursor on the last **visible** line of the filtered document.  
Allow me to completely rephrase the question for you though, and you will most likely stumble upon this problem yourself when answering this question if nothing else:  
Could you please tell me how to write a macro in EmEditor that performs the simple operation of selecting all visible cells in the current column (except the header line) in an arbitrarily filtered document in Cell Selection Mode?  
September 28, 2016 at 1:35 pm [#21086](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/a0a6377144ed3636f985d87303f65ed2?s=80&d=identicon&r=g)Yutaka Emura](https://www.emeditor.com/forums/users/yemura/ "View Yutaka Emura's profile")  
Keymaster  
Hello LifeTimer,  
Thanks for clarification.  
You can use:  
`editor.ExecuteCommandByID(4461);`  
to select the current column without headings.  
Thank you,  
September 28, 2016 at 5:54 pm [#21087](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/21bf85a5da27278c7f73ff85a8eb81ab?s=80&d=identicon&r=g)LifeTimer](https://www.emeditor.com/forums/users/lifetimer/ "View LifeTimer's profile")  
Participant  
Thanks!  
I’d still recommend to implement “real” macro support for it though (e.g. by making the _document.selection.SetActivePoint()_ method optionally be able to use relative visible line numbers instead of only absolute line numbers). :-)  
September 30, 2016 at 3:51 pm [#21093](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/a0a6377144ed3636f985d87303f65ed2?s=80&d=identicon&r=g)Yutaka Emura](https://www.emeditor.com/forums/users/yemura/ "View Yutaka Emura's profile")  
Keymaster  
Hello LifeTimer,  
On the next version (v16.2.0 beta 2), you can use eePosCellView flag to specify the coordinate in Cell View mode. For example:  
`document.selection.SetActivePoint(eePosCellView, 1, 7, false);`  
will set the active cell at (1,7) in the view.  
Thank you,  
September 30, 2016 at 4:09 pm [#21094](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/21bf85a5da27278c7f73ff85a8eb81ab?s=80&d=identicon&r=g)LifeTimer](https://www.emeditor.com/forums/users/lifetimer/ "View LifeTimer's profile")  
Participant  
Excellent, thanks for your responsiveness, as always!
* Author  
Posts

Viewing 9 posts - 1 through 9 (of 9 total)

* You must be logged in to reply to this topic.

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
<li><a href="https://article-files.techidaily.com/new-2024-approved-ultimate-windows-audio-suite/"><u>[New] 2024 Approved Ultimate Windows Audio Suite</u></a></li>
<li><a href="https://desktop-recording.techidaily.com/2024-approved-mastering-your-tech-skills-unlock-macs-full-screen-recording-power-with-shortcuts/"><u>2024 Approved Mastering Your Tech Skills Unlock Mac's Full Screen Recording Power with Shortcuts</u></a></li>
<li><a href="https://facebook-clips.techidaily.com/achieve-social-stardom-the-ultimate-list-for-fb-fan-increase-for-2024/"><u>Achieve Social Stardom The Ultimate List for FB Fan Increase for 2024</u></a></li>
<li><a href="https://win-great.techidaily.com/come-preparare-il-tuo-fissato-la-guida-dettagliata-a-7-metodi-di-masterizzazione-dei-dischi/"><u>Come Preparare Il Tuo Fissato: La Guida Dettagliata a 7 Metodi Di Masterizzazione Dei Dischi</u></a></li>
<li><a href="https://win11.techidaily.com/disabling-corruption-errors-fixing-file-issues-code-0x80070570-on-windows-11/"><u>Disabling Corruption Errors - Fixing File Issues Code 0X80070570 on Windows 11</u></a></li>
<li><a href="https://win-great.techidaily.com/guide-complet-pour-retrouver-des-clips-sms-perdus-techniques-modernes/"><u>Guide Complet Pour Retrouver Des Clips SMS Perdus - Techniques Modernes</u></a></li>
<li><a href="https://android-location.techidaily.com/in-2024-3-effective-methods-to-fake-gps-location-on-android-for-your-realme-12-proplus-5g-drfone-by-drfone-virtual/"><u>In 2024, 3 Effective Methods to Fake GPS location on Android For your Realme 12 Pro+ 5G | Dr.fone</u></a></li>
<li><a href="https://change-location.techidaily.com/in-2024-apply-these-techniques-to-improve-how-to-detect-fake-gps-location-on-poco-c65-drfone-by-drfone-virtual-android/"><u>In 2024, Apply These Techniques to Improve How to Detect Fake GPS Location On Poco C65 | Dr.fone</u></a></li>
<li><a href="https://win-great.techidaily.com/optimierung-der-hyper-v-virtual-machine-leistung-schnelle-losungen/"><u>Optimierung Der Hyper-V Virtual Machine Leistung - Schnelle Lösungen</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/overview-of-the-best-infinix-hot-40-screen-mirroring-app-drfone-by-drfone-android/"><u>Overview of the Best Infinix Hot 40 Screen Mirroring App | Dr.fone</u></a></li>
<li><a href="https://win-great.techidaily.com/problem-mit-outlooks-archivfunktion-die-funf-effektivsten-losungen-fur-nicht-funktionierendes-autoarchivieren/"><u>Problem Mit Outlooks Archivfunktion: Die Fünf Effektivsten Lösungen Für Nicht Funktionierendes Autoarchivieren</u></a></li>
<li><a href="https://win-great.techidaily.com/resolvez-vos-soucis-de-synchronisation-guerir-lerreur-dropbox-smart-sync-en-moins-dune-heure/"><u>Résolvez Vos Soucis De Synchronisation : Guérir L'erreur Dropbox Smart Sync en Moins D'une Heure</u></a></li>
<li><a href="https://extra-skills.techidaily.com/simple-procedure-modify-clownfish-tones-on-pc-for-2024/"><u>Simple Procedure Modify Clownfish Tones on PC for 2024</u></a></li>
<li><a href="https://win-great.techidaily.com/troubleshooting-drag-and-drop-problems-within-textarea-elements-for-emeditor-users/"><u>Troubleshooting Drag-and-Drop Problems Within TEXTAREA Elements for EmEditor Users</u></a></li>
<li><a href="https://instagram-video-files.techidaily.com/visionaries-in-video-top-10-ig-editing-platforms-for-creatives/"><u>Visionaries in Video Top 10 IG Editing Platforms for Creatives</u></a></li>
<li><a href="https://win-great.techidaily.com/1728498778960-windows-11/"><u>Windows 11 ファイル復元ガイド：ファイル履歴機能の活用</u></a></li>
<li><a href="https://win-great.techidaily.com/1728473187573-windows-11/"><u>Windows 11修復輔助程式指南：如何製作隨身碟</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2016129/19272" target="_top" id="2016129">
  <img src="//a.impactradius-go.com/display-ad/19272-2016129" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2016129/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

