<b>English | [中文](./README_zh.md)</b>

<p align="center">
<img src="https://cdn.jsdelivr.net/gh/MoChanBW/DPlayer-ReadyToUse/assets/Cloud_100.png" alt="Cloud-RTU-icon" width="100" >
<img src="https://cdn.jsdelivr.net/gh/MoChanBW/DPlayer-ReadyToUse/assets/anime_character_psyduck.png" alt="d(uck)player-RTU-icon" width="100" ></p>
<h1 align="center">DPlayer-ReadyToUse</h1>

> :dart: Use DPlayer easily with a simple link.

  [![jsDelivr-count](https://img.shields.io/jsdelivr/gh/hm/MoChanBW/DPlayer-ReadyToUse?color=%23e84d3d&logo=jsDelivr&style=flat-square)](https://www.jsdelivr.com/package/gh/MoChanBW/DPlayer-ReadyToUse) [![release](https://img.shields.io/github/v/release/MoChanBW/DPlayer-ReadyToUse?include_prereleases&style=flat-square&logo=Github)](https://github.com/MoChanBW/DPlayer-ReadyToUse/releases/) [![MIT license](https://img.shields.io/github/license/MoChanBW/DPlayer-ReadyToUse?style=flat-square)](https://github.com/MoChanBW/DPlayer-ReadyToUse/blob/master/LICENSE)

## Table Of Content

- [Table Of Content](#table-of-content)
- [Introduction](#introduction)
- [Options](#options)
- [Usage](#usage)
  - [Magnet Link](#magnet-link)
- [Author](#author)

## Introduction

:balloon:**DPlayer-ReadyToUse** is a simple pack to help people use DPlayer more easily.

* :rocket:Using simple URL to access advanced settings for [![DPlayer](https://img.shields.io/badge/Github-MoePlayer%2FDPlayer-FFAF00?logo=Github&style=flat-square)](https://github.com/MoePlayer/DPlayer/)

* :beginner: Using DPlayer in Markdown easily
  
## Options

:white_check_mark:You can custom your player instance with those variables.

:pencil:**Variable Format : Plain Text , unless clearly declared.**

> :arrow_right:[DEMO](https://dplayer.mochanbw.cn/demo/) (stable) [![DEMO on Cloudflare Workers](https://img.shields.io/badge/DEMO%20on-Cloudflare%20Workers-f38020?logo=cloudflare&logoColor=f38020&style=flat-square)](https://dplayer.mochanbw.cn/demo/) [![DEMO Status](https://img.shields.io/uptimerobot/status/m784729343-649b372cd0c06203a3e597ca?label=DEMO%20status&logo=statuspage&logoColor=44CC11&style=flat-square)](https://stats.mochanbw.cn)
>
> :arrow_right:[BETA](https://dplayer.mochanbw.cn/) (slow) [![BETA Status](https://img.shields.io/uptimerobot/status/m784624816-909fad502274ad089ac56ba8?label=BETA%20status&logo=statuspage&logoColor=44CC11&style=flat-square)](https://stats.mochanbw.cn)

|    Name    |            Default            |                                              Description                                              |
|:----------:|:-----------------------------:|:-----------------------------------------------------------------------------------------------------:|
|  autoplay  |             false             |                                    video autoplay , values: 1 , 0                                     |
|  danmaku   |        Wait for update        |                                                                                                       |
|    lang    |      navigator.language       |                                      values: zh-cn , zh-tw , en                                       |
|    live    |             false             |          live mode , values: 1 , 0. Also see [#live](https://dplayer.js.org/guide.html#live)          |
|   magurl   |               -               |                                   see [#Magnet Link](#magnet-link)                                    |
|   picurl   |   [default picurl][picurl]    |                                          url of video poster                                          |
| playerlogo |  'assets/Cloud_alpha_67.png'  |                             url of logo in the top left corner in dplayer                             |
|  preload   |            'auto'             |                            values: none , metadata , auto(wait for update)                            |
|   suburl   |  'assets/demoSubtitle_*.vtt'  |                              external subtitle url (format webvtt only)                               |
|  thumburl  |               -               | video thumbnails, generated by [DPlayer-thumbnails](https://github.com/MoePlayer/DPlayer-thumbnails/) |
|   vidqs    |        Wait for update        |                                                                                                       |
|  vidtype   |            'auto'             |                               values: auto , hls , flv , dash , normal                                |
|   vidurl   | [default video url][videourl] |                                               video url                                               |
|  webicon   |    'assets/Cloud_100.png'     |                                     web icon url(wait for update)                                     |
|  webtitle  |           'DPlayer'           |                                               web title                                               |

## Usage

`/?{Name1}={Value1}&{Name2}={Value2}`

Like this: <https://dplayer.mochanbw.cn/demo/?vidurl=https://t.cn/A6w5s7xn&autoplay=1>

### Magnet Link

Play magnet video based on [![webtorrent](https://img.shields.io/badge/Github-webtorrent%2Fwebtorrent-35B44F?logo=Github&style=flat-square)](https://github.com/webtorrent/webtorrent)

Link Format e.g.`https://yourdomain/?magurl={base64EncodedMagnetLinkHere}`

> :warning: Use base64 encoded Magnet link (charset UTF-8) instead.
>
> :heavy_exclamation_mark: **you should delete all "`=`" at the end of the encoded link before you put it into URL**.

DEMO webtorrent Video: **[Sintel](https://dplayer.mochanbw.cn/demo/?magurl=bWFnbmV0Oj94dD11cm46YnRpaDowOGFkYTVhN2E2MTgzYWFlMWUwOWQ4MzFkZjY3NDhkNTY2MDk1YTEwJmRuPVNpbnRlbCZ0cj11ZHAlM2ElMmYlMmZ0cmFja2VyLm9wZW50cmFja3Iub3JnJTNhMTMzNyZ0cj11ZHAlM2ElMmYlMmZleHBsb2RpZS5vcmclM2E2OTY5JnRyPXVkcCUzYSUyZiUyZnRyYWNrZXIuZW1waXJlLWpzLnVzJTNhMTMzNyZ0cj13c3MlM2ElMmYlMmZ0cmFja2VyLmJ0b3JyZW50Lnh5eiZ0cj13c3MlM2ElMmYlMmZ0cmFja2VyLm9wZW53ZWJ0b3JyZW50LmNvbSZ0cj13c3MlM2ElMmYlMmZ0cmFja2VyLmZhc3RjYXN0Lm56JndzPWh0dHBzJTNhJTJmJTJmd2VidG9ycmVudC5pbyUyZnRvcnJlbnRzJTJm)**

[Online Base64 Encoder(oschina)](https://tool.oschina.net/encrypt?type=3)

[Online Base64 Encoder(base64encode.org)](https://www.base64encode.org/)

> Wait for update

## Author

**DPlayer-ReadyToUse** © [MoChanBW](https://github.com/MoChanBW/). Released under the [MIT License](./LICENSE).

Contribute with [KLPY](https://github.com/KLPY-shuai/)

[picurl]:https://consumer-img.huawei.com/content/dam/huawei-cbg-site/common/mkt/pdp/phones/p40-pro-plus/images/design/design-intro-e-plus.jpg
[videourl]:https://consumer.huawei.com/content/dam/huawei-cbg-site/common/mkt/pdp/phones/p40-pro-plus/images/intro/tvc/video-e-plus.webm
