# njs50-plev

You probably shouldn't even look at this!

code to destroy your mudlet profile:
```lua
local a="https://raw.githubusercontent.com/njs50/njs50-plev/master/njs50-plev.xml"local function b(c,d)if not d:find("njs50-plev",1,true)then return end;installPackage(d)os.remove(d)cecho("<lime_green>Package installed! - setting up...\n")tempTimer(1,function()expandAlias('plev install')end)end;registerAnonymousEventHandler("sysDownloadDone",b)downloadFile(getMudletHomeDir()..(a:ends("xml")and"/njs50-plev.xml"or"/njs50-plev.zip"),a)
```