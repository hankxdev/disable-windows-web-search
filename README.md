# Disable Windows web search 
If you're tired of Windows pushing Cortana and Bing in your face, you're not alone. One of the most frustrating things is seeing web search results and random "search suggestions" whenever you try to use the Start menu to find an app or file.

You hit the Windows key, type a keyword, and instead of just showing your installed programs or local files, it clutters the results with irrelevant junk from the web. If you're here looking for a way to disable this, I bet you think it’s as annoying as I do.

At first, Windows actually let you turn this off through a simple option in the settings. But as more people started disabling it, Microsoft decided to quietly remove the toggle—because, of course, they knew we all hated it.

Now, the only way to turn it off is through Group Policy or by editing the registry. And every time there’s a major update, it’s like starting from scratch.

To save everyone the hassle, I put together a REG file that disables this junk with a single click. It's straightforward, quick, and saves you from having to dig around in settings every time.

Note: I’ve included comments in the REG code itself to make it clear what each part does, in case you’re skeptical or want to verify what’s being changed.

---

`"ConnectedSearchUseWebOverMeteredConnections"=dword:00000000 ` // _disable web search use mobile connection

`"AllowCortana"=dword:00000000`// disable Cortana

`"DisableWebSearch"=dword:00000001` // disable web search

`"ConnectedSearchUseWeb"=dword:00000000` // disabled web searech connection

`"CortanaConsent"=dword:00000000` // disable Cortana

`"BingSearchEnabled"=dword:00000000` // disable bing search in start menu

`"AllowSearchToUseLocation"=dword:00000000` // disable search feature access your location

---
Enjoy :) 
