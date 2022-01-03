# disable-windows-web-search
A reg file to disable Windows shows web search result and search suggestion in Windows search

Windows is promoting its `Cortana` and Bing search. One of the most annoying thing is that it shows web search content when you search in start menu.

So you press `Windows` button, type some keywords, all you want to do is just access your installed app or file quickly, but then you see some shitty stuff in the result list -- web search result and even some so called `search suggesttion`. it's based on your keywords and some trends on the web, since you are searching how to disable this, I know that you also think it's totally garbage. 

In the beginning, Windows gave user an option in the search menu to turn this off. But then Windows knowns that most of the users hated it, so it just removed this option...

I have to use group policy, regeditor to disable it, and have to search for this every time when it updates. 

To do it step by step is a bit complicated and it's totally a waste of time. So I just create this reg file so that anyone who want to do this can do it by one click.

Comment for these reg code in case someone doubt it:

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
