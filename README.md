# cross-screen-live
video live play for computer browser and mobile phone browser

two ways for it.

## one based with xxplayer

how to use:

open the `index.html`:

1. modify something as you need

2. modify `js/live.min.js` with your own live video server:

```js
var vServer = "rtmp://cppfun.com/live";
var vMp4url = "livestream";
var vIosurl = "http://cppfun.com/live/livestream.m3u8";
```

## two based with qcloud video player

how to use:

open the `video.html`:

1. modify something as you need

2. config:

```js
    (function () {
        var player = new qcVideo.Player("id_video_container", {
            "live_url" : "http://yourdomain.com/live/livestream.m3u8", // ios
			"live_url2" : "rtmp://yourdomain.com/live/livestream", // other
			"width" : 640,
			"height" : 480
        });
    })();
```