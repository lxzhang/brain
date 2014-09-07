[M3U]
=====

### Intro

M3U is a computer file format that contains multimedia playlists. 
It originally was designed for audio files, such as MP3, 
but various software now uses it to play video file lists. 
M3U's can also point a media player to an online streaming audio source. 
Numerous media players and software applications supports the M3U file format.


### M3U Samples

Example 1

        #EXTM3U
        
        #EXTINF:123, Sample artist - Sample title
        C:\Documents and Settings\I\My Music\Sample.mp3
        
        #EXTINF:321,Example Artist - Example title
        C:\Documents and Settings\I\My Music\Greatest Hits\Example.ogg

        
Example 2

        C:\Music

        
Example 3

        #EXTM3U
        
        #EXTINF:123, Sample artist - Sample title

        
Example.mp3

        #EXTINF:321,Example Artist - Example title
        Greatest Hits\Example.ogg

Example 4

        Alternative\Band - Song.mp3
        Classical\Other Band - New Song.mp3
        Stuff.mp3
        D:\More Music\Foo.mp3
        ..\Other Music\Bar.mp3
        http://emp.cx:8000/Listen.pls
        http://www.example.com/~user/Mine.mp3

Example 5

        #EXTM3U
        #EXTINF:233,Everclear - So Much For The Afterglow
        Alternative\everclear_SMFTA.mp3
        #EXTINF:227,Weird Al - Everything You Know Is Wrong
        Comedy\Weird_Al_Everything_You_Know_Is_Wrong.mp3
        #EXTINF:187,Weird Al Yankovic - This is the Life
        Weird_Al_This_Is_The_Life.mp3
        #EXTINF:129,Weird Al: Bad Hair Day - Gump
        http://www.site.com/~user/gump.mp3
        #EXTINF:-1,My Cool Stream
        http://www.site.com:8000/listen.pls

* `#EXTM3U` At the VERY top of the Extended M3U file is this header, which signifies this is an extended M3U file. "#EXTM3U" must be all capital letters.
* `#EXTINF:233,Everclear - So Much For The Afterglow`
    * This is the line that tends to confuse people. Let's break it up into parts
    * `#EXTINF`: This signifies this is an Extended Information field. It ends with a colorn.
    * `233`: This is the time of the file in seconds followed by a comma. (233 seconds = 3:53). On the last entry there is a negative one, this is usually seen on streams, it tells the program to ignore the time entry.
    * `Everclear - So Much For The Afterglow`: Title to display. This is usually the title read from the file name or ID3 tags. This also can be the name of a stream. No characters follow the title.
    * `Alternative\everclear_SMFTA.mp3`: File location as described above with basic playlists.     
        

### M3U8

M3U8 is a Unicode UTF-8 version of M3U files for support of Unicode/"international" characters/text. M3U8 follows the same principles as explained above.

Example

        #EXTM3U
         
        #EXT-X-STREAM-INF:PROGRAM-ID=1,BANDWIDTH=1217000,RESOLUTION=1280x720
        2013girlwithipad-1200k.m3u8
         
        #EXT-X-STREAM-INF:PROGRAM-ID=1,BANDWIDTH=824000,RESOLUTION=896x504
        2013girlwithipad-800k.m3u8
         
        #EXT-X-STREAM-INF:PROGRAM-ID=1,BANDWIDTH=629000,RESOLUTION=640x360
        2013girlwithipad-600k.m3u8
         
        #EXT-X-STREAM-INF:PROGRAM-ID=1,BANDWIDTH=430000,RESOLUTION=512x288
        2013girlwithipad-400k.m3u8
         
        #EXT-X-STREAM-INF:PROGRAM-ID=1,BANDWIDTH=216000,RESOLUTION=400x300
        2013girlwithipad-200k.m3u8
         
        #EXT-X-STREAM-INF:PROGRAM-ID=1,BANDWIDTH=121000,RESOLUTION=400x300
        2013girlwithipad-110k.m3u8

		
---

**See also**

* [draft-pantos-http-live-streaming-08 - HTTP Live Streaming](http://tools.ietf.org/html/draft-pantos-http-live-streaming-08)


**Refs**

* [M3U - Wikipedia, the free encyclopedia](http://en.wikipedia.org/wiki/M3U)
* [M3U Play List Specification - The Schworak Site](http://schworak.com/blog/e39/m3u-play-list-specification/)
* [M3U and PLS Specification - Winamp Forums](http://forums.winamp.com/showthread.php?threadid=65772)
* [What is an .M3U8 file? m3u8 template - GravityLab](http://www.gravlab.com/2013/07/05/what-is-an-m3u8-file/)
* [PLS (file format) - Wikipedia, the free encyclopedia][PLS]


[PLS]: http://en.wikipedia.org/wiki/PLS_(file_format)
[M3U]: https://gist.github.com/district10/a982f999a7e853d3ca1b