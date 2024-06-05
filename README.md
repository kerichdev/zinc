# zinc
best way to save what you love: [zinc.kerichuu.space](https://zinc.kerichuu.space/)  

![zinc logo banner](/src/front/icons/pattern.png "zinc logo banner")

## what's zinc?
zinc is a fork of [cobalt](https://https://github.com/imputnet/cobalt) - a media downloader that doesn't piss you off. it's fast, friendly, and doesn't have any bullshit that modern web is filled with: ***no ads, trackers, or invasive analytics***.  

paste the link, get the file, move on. it's that simple. just how it should be.

## supported services
this list is not final and keeps expanding over time.

| service                        | video + audio | only audio | only video | metadata | rich file names |
| :--------                      | :-----------: | :--------: | :--------: | :------: | :-------------: |
| bilibili.com & bilibili.tv     | ✅            | ✅         | ✅         | ➖         | ➖              |
| dailymotion                    | ✅            | ✅         | ✅         | ✅         | ✅              |
| instagram posts & reels        | ✅            | ✅         | ✅         | ➖         | ➖              |
| loom                           | ✅            | ❌         | ✅         | ✅         | ➖              |
| ok video                       | ✅            | ❌         | ✅         | ✅         | ✅              |
| pinterest                      | ✅            | ✅         | ✅         | ➖         | ➖              |
| reddit                         | ✅            | ✅         | ✅         | ❌         | ❌              |
| rutube                         | ✅            | ✅         | ✅         | ✅         | ✅              |
| soundcloud                     | ➖            | ✅         | ➖         | ✅         | ✅              |
| streamable                     | ✅            | ✅         | ✅         | ➖         | ➖              |
| tiktok                         | ✅            | ✅         | ✅         | ❌         | ❌              |
| tumblr                         | ✅            | ✅         | ✅         | ➖         | ➖              |
| twitch clips                   | ✅            | ✅         | ✅         | ✅         | ✅              |
| twitter/x                      | ✅            | ✅         | ✅         | ➖         | ➖              |
| vimeo                          | ✅            | ✅         | ✅         | ✅         | ✅              |
| vine archive                   | ✅            | ✅         | ✅         | ➖         | ➖              |
| vk videos & clips              | ✅            | ❌         | ✅         | ✅         | ✅              |
| youtube videos, shorts & music | ✅            | ✅         | ✅         | ✅         | ✅              |

| emoji   | meaning                 |
| :-----: | :---------------------- |
| ✅      | supported               |
| ➖      | impossible/unreasonable |
| ❌      | not supported           |

### additional notes or features (per service)
| service    | notes or features                                                                                                    |
| :--------  | :-----                                                                                                               |
| instagram  | supports reels, photos, and videos. lets you pick what to save from multi-media posts.                               |
| pinterest  | supports photos, gifs, videos and stories.                                                                           |
| reddit     | supports gifs and videos.                                                                                            |
| rutube     | supports yappy & private links.                                                                                      |
| soundcloud | supports private links.                                                                                              |
| tiktok     | supports videos with or without watermark, images from slideshow without watermark, and full (original) audios.      |
| twitter/x  | lets you pick what to save from multi-media posts. may not be 100% reliable due to current management.               |
| vimeo      | audio downloads are only available for dash.                                                                         |
| youtube    | supports videos, music, and shorts. 8K, 4K, HDR, VR, and high FPS videos. rich metadata & dubs. h264/av1/vp9 codecs. |

## zinc api
zinc has an open api that that i use in my projects. it's easy and straightforward to use, [check out the docs](/docs/api.md) if you want to drop in as well.

✅ you can use the main api instance ([bazinca.kerichuu.space](https://bazinca.kerichuu.space/)) in your **personal** projects, do drop me a message about doing so.

## ethics and disclaimer
zinc is a tool for easing content downloads from internet and takes ***zero liability***. you are responsible for what you download, how you use and distribute that content. please be mindful when using content of others and always credit original creators. fair use and credits benefit everyone.

zinc is ***NOT*** a piracy tool and cannot be used as such. it can only download free, publicly accessible content. such content can be easily downloaded through any browser's dev tools. pressing one button is easier, so i made a convenient, ad-less tool for such repeated actions.

## zinc license
zinc code is licensed under [AGPL-3.0](/LICENSE).

zinc branding, mascots, and other related assets included in the repo are ***copyrighted*** and not covered by the AGPL-3.0 license. you ***cannot*** use them under same terms.  

## 3rd party licenses
- [Fluent Emoji by Microsoft](https://github.com/microsoft/fluentui-emoji) (used in zinc) is under [MIT](https://github.com/microsoft/fluentui-emoji/blob/main/LICENSE) license.  
- [Noto Sans Mono](https://fonts.google.com/noto/specimen/Noto+Sans+Mono/) fonts (used in zinc) are licensed under the [OFL](https://fonts.google.com/noto/specimen/Noto+Sans+Mono/about) license.  
- many update banners were taken from [tenor.com](https://tenor.com/).  

## acknowledgements
### cobalt, obviously
[cobalt](https://https://github.com/imputnet/cobalt) is the project zinc is forked and rebranded from, and the licence requires i mention them, albeit i'd do that anyway since its a cool project. 

### ffmpeg
zinc heavily relies on ffmpeg for converting and merging media files. it's an absolutely amazing piece of software offered for anyone for free, yet doesn't receive as much credit as it should.

you can [support ffmpeg here](https://ffmpeg.org/donations.html)!

#### ffmpeg-static
we use [ffmpeg-static](https://github.com/eugeneware/ffmpeg-static) to get binaries for ffmpeg depending on the platform.

you can support the developer via various methods listed on their github page! (linked above)

### youtube.js
zinc relies on [youtube.js](https://github.com/LuanRT/YouTube.js) for interacting with the innertube api, it wouldn't have been possible without it.  

you can support the developer via various methods listed on their github page! (linked above)

### many others
zinc also depends on:

- [content-disposition-header](https://www.npmjs.com/package/content-disposition-header) to simplify the provision of `content-disposition` headers.
- [cors](https://www.npmjs.com/package/cors) to manage cross-origin resource sharing within expressjs.
- [dotenv](https://www.npmjs.com/package/dotenv) to load environment variables from the `.env` file.
- [esbuild](https://www.npmjs.com/package/esbuild) to minify the frontend files.
- [express](https://www.npmjs.com/package/express) as the backbone of zinc servers.
- [express-rate-limit](https://www.npmjs.com/package/express-rate-limit) to rate limit api endpoints.
- [hls-parser](https://www.npmjs.com/package/hls-parser) to parse `m3u8` playlists for certain services.
- [ipaddr.js](https://www.npmjs.com/package/ipaddr.js) to parse ip addresses (for rate limiting).
- [nanoid](https://www.npmjs.com/package/nanoid) to generate unique (temporary) identifiers for each requested stream.
- [node-cache](https://www.npmjs.com/package/node-cache) to cache stream info in server ram for a limited amount of time.
- [psl](https://www.npmjs.com/package/psl) as the domain name parser.
- [set-cookie-parser](https://www.npmjs.com/package/set-cookie-parser) to parse cookies that zinc receives from certain services.
- [undici](https://www.npmjs.com/package/undici) for making http requests.
- [url-pattern](https://www.npmjs.com/package/url-pattern) to match provided links with supported patterns.

...and many other packages that these packages rely on.
