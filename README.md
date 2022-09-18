# zingmp3py
#### A light weight Python library for the ZingMp3 API
##### *all functions are return dict or ZingMp3 Object

# Sync :
```py
from zingmp3py import ZingMp3

zi = ZingMp3()
zi.getDetailPlaylist("67ZFO8DZ")
zi.getDetailArtist("Cammie")
zi.getRadioInfo("IWZ979CW")
zi.getSongInfo("ZWAF6UFD")
zi.getSongStreaming("ZWAF6UFD")
zi.getTop100()
zi.search("rick roll")
```

# Async
```py
import asyncio
from zingmp3py import ZingMp3Async

async def main():
    zi = ZingMp3Async()
    await zi.getDetailPlaylist("67ZFO8DZ")
    await zi.getDetailArtist("Cammie")
    await zi.getSongInfo("ZWAF6UFD")
    await zi.getSongStreaming("ZWAF6UFD")
    await zi.getTop100()
    await zi.search("rick roll")

loop = asyncio.get_event_loop()
loop.run_until_complete(main())
```

## Get Type And ID

```py
from zingmp3py import getUrlTypeAndID

getUrlTypeAndID("https://zingmp3.vn/liveradio/IWZ979CW.html")
```
