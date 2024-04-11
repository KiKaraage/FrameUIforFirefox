# Welcome to my fork of FrameUIforFirefox!
Original theme by FineFuturity. Tweaks by [MrOtherGuy/firefox-csshacks](https://mrotherguy.github.io/firefox-csshacks/), [bmFTzQ/Edge-Frfox](https://github.com/bmFtZQ/edge-frfox) & [Shina-SG/Shina-Fox](https://github.com/Shina-SG/Shina-Fox). Fork & modifications by KiKaraage.  *(Issues, questions or feedbacks can be submitted here or in [Reddit](https://old.reddit.com/r/FirefoxCSS/comments/1bzos14/presenting_my_version_of_frameui_for_firefox/))*

## Additional features:
* Optimization for compact mode, devices with smaller screens: smaller icons scale, smaller & centered URL font size, stripped URL bar background.
* Fluent icons & Ms Edge-like hamburger menu/context menu styling (derived from Edge-Frfox).
* Pop-up searchbar (derived from Shina-Fox) | Enable by adding new Boolean preference in `about:config`: `uc.tweak.popup-search`
* Multi-panel Sidebery setup | Enable by putting codes from [sidebery-css-style](https://github.com/KiKaraage/ArcWTF/blob/main/sidebery-css-style) onto the Sidebery styles editor.
* **Update 1**: Enabling frame configuration for true Polaroid experience | Enable by adding new Boolean preference in `about:config`: `uc.tweak.frame` *(You can also adjust rounded corner radius in ~line 1125 of the userChrome)*
* **Update 1**: To enable autohidden sidebar, you can replace codes in "D) SIDEBAR" section, after line 948, with [this code](https://github.com/KiKaraage/ArcWTF/blob/main/tweaks/sidebar.css) while installing Userchrome Toggle altogether (you can refer to [ArcWTF readme]([h](https://github.com/KiKaraage/ArcWTF)) for clearer setup tutorial on UCT).
* Suggested addons to use: [Adaptive Tab Bar Color](https://github.com/easonwong-de/Adaptive-Tab-Bar-Colour) for adaptive theming | [Gesturefy](https://github.com/Robbendebiene/Gesturefy) for easier page navigations, less clicks | [MaxFocus Link Preview](https://addons.mozilla.org/en-US/firefox/addon/maxfocus-link-preview/reviews/), alternatives to Peek features in Arc Browser
* Font used in screenshots: Google Sans Text | Add on your userChrome/userContent: `* {font-family: "Google Sans Text" !important;}
`

![Screenshot 1, general look](https://github.com/KiKaraage/FrameUIforFirefox/assets/10529881/42e42d1f-8830-442a-8e64-b725cd6da508)
![Screenshot 2, pop-up searchbar](https://github.com/KiKaraage/FrameUIforFirefox/assets/10529881/9f35fee2-a9b4-477c-9747-8d01d3978eb5)
![Screenshot 3, main Firefox menu](https://github.com/KiKaraage/FrameUIforFirefox/assets/10529881/928fbe4c-573f-45ba-bb20-a6d514742b13)
![Screenshot 4, with frame config enabled](https://github.com/KiKaraage/FrameUIforFirefox/assets/10529881/c5f21506-6d36-4485-a479-26a5f652ac66)


# Codename: FrameUI For Firefox
A new way to view your web content, like looking at photos printed from an old Polaroid camera.

![a1fd4499dd2be9a2ecccc660a6ce0696](https://github.com/FineFuturity/FrameUIForFirefox/assets/19298107/75c5a475-d440-4481-a002-9cdb754155ed)

# Changelog
```
Version 0.3a:
* The latest Firefox update caused some issues with clicking on interface elements, including the window controls.  The latest update to the theme fixes this issue.
  * I'm not sure if the update caused any other issues, so please report them as you see them.  
* Fixed the alignment of the private browsing indicator when in private browsing mode.
 

Version 0.3:
* Better support for configurations where the title bar buttons are either on the left or right side of the window, regardless of OS.
  * HUGE thanks to MrOtherGuy's CSS ![code](https://github.com/MrOtherGuy/firefox-csshacks/blob/master/chrome/toolbars_below_content.css), without which I would not have been able to fix this as well as the below issues.
* Fixed issues with the menubar not playing nicely with the navigation bar when it's active.
* Fixed issue with the private browsing indicator icon being misaligned with the navigation bar when in private browsing mode.
* Fixed issue where the bookmarks toolbar would push the navigation toolbar past the bottom window boundary if "Only Show on New Tab" was set.
* When clicked, the address bar's URL text now stays at the bottom rather than moving to the top.
  * This should make typing a URL or search term much less jarring.


Version 0.2:
* Initial macOS support.
  * Platform detection has been added, so the theme now accounts for configurations where either the title bar buttons are on the left (e.g., macOS/Linux title bar buttons on left) or on the right (e.g, Windows/Linux title bar buttons on right).
* Fixed issue with user-selected themes either working inconsistently or not at all.
* Inactive window title bars are now darker to differentiate them from the active window.
 
Version 0.1:
* Initial release
```


**macOS NOTE:**
* FrameUI was designed to have the window control buttons on the bottom. However, due to the way that fullscreen windows work on macOS, the window control buttons will remain at the top of the window like other macOS apps. This complication is not present in windowed mode.

# Prerequisites
* For this to work, make sure `toolkit.legacyUserProfileCustomizations.stylesheets` and `svg.context-properties.content.enabled` is set to `true` in `about:config`.
* To make the most of this theme, it is **STRONGLY recommended** that you install an addon for vertical tabs, such as Tab Center Reborn.  **This is a stopgap for now until I figure out how to integrate native vertical tab functionality into the theme.**
* If you're on Linux, make sure your window controls are set to be on the right side of your title bar.

# Installation

Simply drop the provided `userChrome.css` file into your `chrome` folder and restart for the changes to take effect.

# Motivation
_(by FineFuturity)_ After restarting, you'll notice that *all* of the controls -- the navigation bar, the window controls, *everything* -- has been moved to the bottom in a manner reminiscent of the Metro-based Internet Explorer app seen in Windows 8/8.1.  While I think Microsoft was on the right track with their attempts at a tablet-based interface... well, we all know what happened.  Apart from Microsoft's attempt at a touch interface (which was a half-done attempt anyway), I think no company to this day has yet to get right.

This theme is a step towards what I believe may solve the grand problem of unifying the desktop and tablet interface for ANY device form factor.  What I hope you'll find is that this interface works really well on *both* tablet and desktop form factors, precisely because there is no longer a need for a user to lift their arms to get to something as basic as the window controls -- they're now just a mere finger reach away. 
