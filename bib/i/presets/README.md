#settings
* google translated from japanese

Preset specified manual 2016/04/21 Edition
It is easy, but it describes the preset. Because it is a plan to put together in the future manual, please forgive often reads Zura is.

Preset A / how to use

Preset file is a text file that is outside the initial setting of the default behavior and layout of as a reader. You can customize the Bibi by editing this. (Format, reality or rather is the object of JavaScript)

You use to put on bib / i / presets / folder. But, even in the matter of fact somewhere else (also elsewhere server) it does not matter.

bib / i / index.html of the state in which the distribution is calling a bib / i / presets / default.js. By changing this, you can change the preset you want to use. bib / i / index.html also, for example, it is possible to selectively use to copy, rename as bib / i / the-great-book.html, mean that it is possible to selectively use a combination of HTML and presets for each book is.

For customization, at the beginning

Or less, but describes the specific designation that you can customize the behavior, many, there are advantages and disadvantages by EPUB of interest. That's why, not fixed uniformly at the Bibi side, I mean that are to be edited as a preset.

But there are also items that can be changed in the button while reading it yourself, or if you want to show the EPUB that you created on your own to the reader, such as when I want to use the BiB / i you customize the look and feel on your own to the reader, to EPUB When specified in the combined style and pre-preset like you style, I think that it is certainly nice.

Definitions of terms used in this document

An item is a file one by one to be displayed.

The "spread" is a block wrapping the item. Reflow specified items will constitute the "spread" in only one it. If the left and right pairs at a fixed layout has been made, although two that will enter the one "spread".

"Length", is the direction of travel size. Left and right width when you are traveling in a horizontal direction, refers to if the vertical up and down height. Similarly, "breadth" is, up and down high if horizontal progression, is if the vertical left and right width. And, then those numbers are small state to be referred to as "short", "narrow".

These definitions are not necessarily being used in general for the EPUB or e-book, please I think the only Bibi term.

Item Description 1: definition section

Does not affect the behavior and display, is the definition of a preset file itself.

Does not have also been used anywhere at the moment, but Shirezu may put a function of switching a preset from someday control panel, is scheduled is to be used as a label or description in the configuration panel to the Akatsuki.

"Preset-name": any name of "name" ... preset

"Preset-description": "description" content of ...... preset description

"Preset-author": "author" ... preset of the author's name

"Preset-author-href": a link to the "URI" ...... preset author

Item Description 1: Basic Configuration

You control the very basic behavior of Bibi.

Path to the "bookshelf" ...... bookshelf directory

To describe the path of bib / / index.html seen from the bookshelf directory. The same relative path root relative path to the bookshelf directory of the web server ( "../bookshelf/" Ya "/ bib / bookshelf /", etc.) does not matter.

As an advanced setting, http the bookshelf directory of the server on which the cross-origin request is permitted (s): You can also write from //. However, the origin of the server, must be included in the end to describe "trustworthy-origins" of this document.

"Reader-view-mode" initial value of ...... display mode (page-turning, horizontal scroll vertical scrolling)

Page-turning mode If you specify a "paged", side-scrolling mode if "horizontal", to start the display in the vertical scroll mode if "vertical". Because the reader can be changed at any time, or to display only the first in any mode, is that.

"Fix-reader-view-mode" to fix the ...... display mode whether to prevent the change

"Yes", "no", "desktop", you can choose from four of the "mobile". Or later, but this four specified appeared some, it is the same switching conditions.

The initial value of this item is "no", we recommend that you leave that. Always When "yes", "desktop" if the time of the personal computer, at the time of the "mobile" if smart phone, the user will not be able to change the display mode, you will not also appear change button. Better to ban depending on the nature of the content will use when it is to improve the user experience.

"Autostart" ...... when pasted, whether to open automatically this without waiting for the click of the play button

Bibi but you can use embedded in a web page, and automatically play a large book of the amount of data, you might tend to slow down the process of reading the parent web page.

That said, you do not might want would be if light the automatic playback, you may want to switch the behavior in the personal computer and the smartphone.

So this also, "yes", "no", "desktop", with the value of the "mobile", was as to be switched. If "yes", also always autoplay any time. "No", on the other hand, requires a click / tap the play button always. "Desktop" is, auto-play if the personal computer, the smart phone will require the operation of the play button. "Mobile" is the opposite of "desktop".

"Start-in-new-window" when you press the play button in the ...... Paste state, whether to open in a new window

If the time of paste, the play button depending on the setting of the "autostart" is displayed, when you click / tap the Play button, or to play with as it is paste state, is whether the set open in a new window.

This is also "yes", "no", "desktop", "mobile" have become to choose from 4-necked, "yes" is always another window, "no" is always embedded state, "desktop" is if the personal computer embedded if smartphone in a separate window, "mobile" is the opposite, the "desktop".

Until very recently, Bibi was the same behavior as always "mobile". I desire to start remains embedded in smartphone I had here and there, but a sufficient performance did not appear to read.

But, since it seems like began to move soon decent, you have to choose at any. However, in the case of a smart phone, it may force the inconvenience to the reader when opened in a smaller frame of the narrow screen. Please try using care well. (The user can fix open from the button in the menu at any time another window. That said)

Or use the "use-slider" ...... page slider

When you click / tap the per the middle of the screen is the presence or absence of use of the page slider to come out at the lower end. In a convenient UI that you can jump to the desired position in the book, and is enabled, in the personal computer and also serves as the role of the pseudo-scroll bar at the time of the page turning mode. This is also the setting of "yes", "no", "desktop", "mobile", the initial value is "yes".

Or "use-arrows" page to react to click / tap of ...... the edge of the screen turning using a function

Bibi is to prepare the page-turning area to the left and right screen, it can now be operated by click / tap. However, when you or they are no longer needed with the own UI to the parent page or app embedded formed a special program, and listed as erasable. This is also the setting of "yes", "no", "desktop", "mobile", the initial value is "yes". Since this a most cases would no longer turned up that there is no, basically we recommend leave the "yes".

Or accept the "use-keys" ...... keyboard operation

When enabled, you can page also move with the cursor keys on the keyboard. This is also the setting of "yes", "no", "desktop", "mobile", the initial value is "desktop". Since the function can not be used in smartphone enabled, we recommend the "desktop" or "no".

Or turn over in drag / swipe at the time of the "use-swipe" ...... page turning mode

When enabled, you will be turning swipe at the page-turning mode can be used. This is also the setting of "yes", "no", "desktop", "mobile", the initial value is "yes". However, if this is enabled, you will not be able to select the text in the page-turning mode. In the personal computer, quickly but will work with the release and drag it to the left and right, it might be good to set to "no" Ya "mobile" when you think that it will not do the operation on a PC. (But, I think I am sometimes and try to the user test, and its operation is also a PC person)

"Use-cookie" to save ...... state to Cookie or to reproduce in the next time you open

When enabled, the display mode is saved and page position when that was last opened, the same book will start in the same state the next time. To a particular book, the combination of the present ID that was written in Bibi directory and EPUB meta file (identifier) ​​is used. This is also the setting of "yes", "no", "desktop", "mobile", the initial value is "yes". Since the reason to separate the behavior in the personal computer and the smartphone would not particularly, please choose on whether "yes" or "no". Only the display mode and page position to be recorded, but does not leak or private information to the outside by this feature.

Expiration date of when you save a "cookie-expires" ...... Cookie (in seconds)

Expiration date of when the Cookie is saved to enable the "use-cookie" above. Unit is in seconds, the initial value is 60 * 60 * 24 * 3. In this sense that the 60 × 60 × 24 × 3, 1 hour at 60 times of 60 seconds, one day in the 24-fold, because the three times that, that has become a 3 days. The same thing even need to mention 259200 of pre-multiplied value, but, how is easy to understand better to rose, and. I think that long and keep you in a few days is good. For example, reading only the middle of a reload in a few minutes about if you want to support, please try and so on.

"Ui-font-family" ...... Table of Contents and the font specification of other basic UI

CSS of the font-family can be specified as such. For example, you want to use that kind of font because the font you place the punctuation marks in the box center in Taiwan is generally, when there are circumstances, such as such, you can specify a default font.

Notes of you, but this does not affect the body. Only, font, such as table of contents to be displayed as Bibi function of.

Item Descriptions 2: display customize book content

"Book-background" ...... under the "spread" background

Behind the white box of the "spread", there is a dark color area. You can change the bottom of the style. CSS of background please leave that. That can also be used, such as the background image.

"Spread-gap" ...... as the "spread" interval of the "spread"

The interval between the "spread" of reflow content. Unit is px.

Distance of the first and last of the window end "spread" is, this value regardless, will be adjusted the distance between the window end to come in the middle of the window.

Also, in the case of a fixed-layout is automatically adjusted regardless of this value.

"Spread-margin" interval of ...... as "spread" window

Of the window as the "spread" at the time of the scroll mode, is the interval of the "width" direction (traveling direction and vertical axis of the book). Unit is px. When the page-turning mode, this value is ignored stick exactly to the window.

"Spread-margin-start" is, when the horizontal scroll mode up and down, when the vertical scroll mode is left and right.

"Spread-border-radius" ...... Kado round setting of "spread"

Of that you can now with CSS 3, there is a legend that many of the author was most clearly dancing for joy, it is Kado circle specified. You can round the excessive white box of the "spread". CSS of border-radius as it is, please your liking.

The CSS if put a shadow on the "spread-box-shadow" ...... "spread"

Arranged in Kad round reportedly spoke with was dancing for joy the authors, drop shadow. It will be shaded in white box of the "spread". CSS of box-shadow is as it is.

Because you might limp a little scroll and add shadows, it might be better not. Please be unnecessary if "none" or "".

"Item-padding-left" / "* -right" / "-top" / "*** - bottom" ...... margin within each item

Is the margin of the area where the inside, each HTML in the EPUB is drawn in the "spread". All units of the numerical value px (pixels).

Croaker you, but ...... really is I think or not it should say a total of 0. If the author can be controlled by the CSS in EPUB, because should that person is good.

But, iBooks beginning, leading the system to put the uncontrolled margin has dominated the width. Together with such leading system, EPUB you have narrowed or not to set the margin is quite large. This item is for that.

Applied background color and background image to HTML in the EPUB also processed as is reflected in this margin. However, this is ignored when the fixed layout, the margin adjustment by BiB / i does not take place.

"Page-breaking" whether or not to enable ...... page break specified [corresponding incomplete]

If true, the page break by the page-break-before and page-break-after of the CSS. The initial value is false.

...... But, it does not move well. We recommend that you leave the false.

Add any of the CSS / JavaScript content in the "epub-additional-stylesheet" / "epub-additional-script" ...... EPUB

Without having to edit the content in the EPUB, you can add a CSS / JavaScript on all of the items. Want to check the display to add the script for and verification and calibration you want to read at your own style, it is the ability to meet the needs of such.

The value you specify as it is the path. However, there is a case that does not work by the various constraints of the browser and the server.

Description of item 3: Extension

The Bibi, you have a mechanism that can extend the functionality by adding another file in bib / i / extensions / are available. Such mechanism is generally plug-ins, extensions, but it is said with such enhancements, we have to be referred to as an extension in the Bibi (Bibi is because the girl, it would be nice to ish accessory?).

Extensions that are shipped at the time of distribution is five. Among them, only Unzipper is enabled by default.

Basic extension

For example, suppose you have got a new extension named Example.

Since the extension has become in the folder structure that example / example.js, first, put the example folder in bib / i / extensions / folder.

Then, in the next line of the line that begins with the preset of "extensions", { "name": "Example", "src": "extensions / example / example.js"}, you add written as such. You should see if there is a designation from the author of the always should add to write extensions. Yes by adding write to all the bundled extensions default.js, Sonouede, what you want to disable by default I've commented out.

Then, Bibi read in add the extension at startup, the function of the extension is enabled.

The following describes the bundled extension.

"Unzipper" not ...... deployed to handle the (= Zip archived) EPUB

Enabled by default. However, because it is not lodged by the restriction in Internet Explorer, it does not effective even nothing.

EPUB has been archived in Zip format, the browser is usually can not handle files that are in the interior of the Zip archive. By this extension, Bibi will be able to handle even EPUB archive state.

However, since Bibi by the received PC / smart phone needs to be processed to expand, from around the file size EPUB exceeds 10MB, the length of processing time to begin reading is becoming conspicuous. The first place because the heavy and further expand the consuming file transfer time, is that there is no way. Also, I do not is a big difference in the speed of operation Once you have displayed once, such as in the old and less powerful smart phone, you may get stuck is Bibi previously displayed in the processing load of the deployment. In addition, there is a limitation of function in Internet Explorer, you can not open a book of Zip state in Bibi even with this extension.

So, when you publish a book with the Bibi, we recommend that you pre-deployment. Although this extension I was thinking whether'll keep the disabled in the initial value, the first place the initial development is rather in the basic functions of Bibi much can not be handled only by the remains of the archive state, also, the compressed file in the drag-and-drop also the open, is a useful Bibi benefits, such as in the preview of your own EPUB. By default Yes to enable the why.

Since this extension is a reasonable file size, I think that is also good to keep the disabled If you do not use only deployed this. The amount of data to be read is made lightly, as a result, a little only, time to be able to operate this may become shorter. I said, I is the size that does not reach even 1 photo of nowadays with. Also effective, but there is no longer a process itself to open a deployed this slow.

You will be able to analyze the behavior of the user in the "Analytics" ...... Google Analytics

It is enabled by default. However, "tracking-id" in the Google Analytics tracking ID (format: UA-XXXXXXXX-X) unless the write added together, do nothing.

When it comes to publish a book on the web, how many people is whether you click the Play button, or was clicked which item in the table of contents, or have read to the end, and so, I think that will come in the mood. These are, so that you can record using the event tracking features of Google Analytics. To fit well as OS and access the original language zone to be recorded at the same time as the basic functions of Google Analytics, you will be a read the situation can be different analysis.

The current is recorded, is the user action listed below. If you have anything you would like to record and analyze In addition, please request more and more to the author.

Play button of the click / tap
An entry in the table of contents click / tap
Display of the last page
You will be able to share "Share" ...... the URL of Bibi URL or embedded parent page that is open the book to the SNS

It is enabled by default.

The book itself, nor the parent page that has been embedded, you will be get to share the URL to Twitter / Facebook / Google+.

To be able to use the position and range specification of "EPUBCFI" ...... EPUBCFI specification

It is disabled by default.

EPUBCFI is, in the EPUB composed of multiple files, is a mechanism that allows you to specify what what th character from the character position, such as position and range of a particular paragraph of a particular file. Makes it easier to or communicated to the people in the link, such as "this about this is written here in this book." It can also be used, such as paper of reference.

EPUB viewer is desirably correspond to EPUBCFI, because it is convenient if you use the actual well or Bibi also partially corresponding How can ...... format tried it because it felt that "It 's not something that can be human to read and write", specification itself There are not used much. This plug-in is also fully compatible give up of features that have been prepared to the specifications, we stopped developed in response only to the specified position (not handle the range specification).

So, by default, Yes to turn off and commented out, does not this extension is read. Please remove the comment out when you want to enable.

The Bibi, Yes wearing a separate function to open by specifying in the middle of a book without using EPUBCFI. It is a unique feature, not the basic specifications of EPUB, but can now be specified in a more straightforward simple formatting. Because it is a separate commentary plans, Fun to.

So the reflow version can overlay displayed on the book "OverReflow" ...... fixed layout

It is disabled by default.

Since this is an extension of fairly developers, and omit the description. People who thought, "interesting" in the example used below, please ask you a question directly. The EPUB itself we need to make for this plug-in, but once, within the range that is allowed in the EPUB specification.

Example of use: https://pan.press/sinap/journal/SINAP-Journal_Summer-2015/

Adjust the typesetting of "JaTEx" ...... Japanese vertical writing reflow content

It is disabled by default.

It was named in the stands for Japanese Typesetting Extra. Japanese typesetting expansion, means such. Automatic mark-up and of parentheses enclosing scope and about things, provides automatic control, such as hanging punctuation. How to use it is difficult, if not finely tuned together with the making of the book, have a significant impact on the operating speed. Since this is also an extension of fairly developers, and omit the description.

Example of use: https://pan.press/seikaisha/fictions/sekaisouzou-kabushikigaisha-1/

Item Description 4: (It is recommended that you do not change as long as the common use) Advanced Settings

Origin to allow as "trustworthy-origins" ...... bookshelf installation location and Message source of

If necessary By enumerating the external origin, or place a bookshelf to the external server, you will be able to or receive an operation instruction in the Message from another server. Without writing anything, the origin of the server that Bibi itself is placed will be allowed.

For example, If you add the "https://dl.dropboxusercontent.com" here, you will be able to or read EPUB of Dropbox from your web server. However, it will be able to also be used in order to display the EPUB someone has put in Dropbox shared folder of the people who do not know at all.

With caution, all of the following documents routes I think that is good to add the only server that is under your control.
