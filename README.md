<b>English | [中文](https://github.com/MoChanBW/DPlayer-ReadyToUse/blob/master/README_zh.md)</b>

<h1 align="center">DPlayer-ReadyToUse</h1>

> Use DPlayer easily with a single link.

 [![MIT license](https://img.shields.io/github/license/MoChanBW/DPlayer-ReadyToUse)](https://github.com/MoChanBW/DPlayer-ReadyToUse/blob/master/LICENSE)

## Introduction

<div style="position: relative; width: 98%; height: 100%; box-sizing: border-box; margin:auto;padding:0;">
<iframe src="https://dplayer.mochanbw.cn" seamless scrolling="no"  frameborder="0"  allowfullscreen="true" style="position: absolute; width: 100%; height: 100%; "></iframe>
</div>

*DPlayer-ReadyToUse* is a simple pack to help people use DPlayer more easily.

* Using simple URL to access advanced settings for [DPlayer](https://github.com/MoePlayer/DPlayer).

* Using DPlayer in Markdown easily.

## Options

You can custom your player instance by those variables.

> DEMO : <https://dplayer.mochanbw.cn/>

|    Name    |          Default           |                                                         Description                                                          |
|:----------:|:--------------------------:|:----------------------------------------------------------------------------------------------------------------------------:|
|  autoplay  |           false            |                                                video autoplay , values: 1 , 0                                                |
|  danmaku   |      Wait for update       |                                                                                                                              |
|    live    |           false            |                  enable live mode, values: 1 , 0. Also see [#live](https://dplayer.js.org/guide.html#live)                   |
| magneturl  |      wait for update       |                                                      base64 encoded url                                                      |
|   picurl   |   see [#defaultPicurl]()   |                                                         video poster                                                         |
| playerlogo |      Wait for update       |                                             showing logo in the top left corner                                              |
|   suburl   | 'asset/demoSubtitle_*.vtt' |                                                                                                                              |
|  thumburl  |            true            |             video thumbnails, generated by [DPlayer-thumbnails](https://github.com/MoePlayer/DPlayer-thumbnails)             |
|   vidqs    |      Wait for update       |                                                         (Maybe Not)                                                          |
|  vidtype   |           'auto'           | values: auto , hls , flv , dash , normal , <b>webtorrent</b>*(Need base64 encoded and can't use in 'auto')*(wait for update) |
|   vidurl   |   see [#defaultVidurl]()   |                                                          video url                                                           |
|  webicon   |      Wait for update       |                                             Configure web icon , value :  string                                             |
|  webtitle  |         'DPlayer'          |                                            Configure web title , value :  string                                             |

## Usage

`/?[Name1]=[value1]&[Name2]=[value2]` etc.

> Wait for update

## Why create this repo

> I WAS A REAL NOOB WHEN I FIRST USED DPLAYER.
> Official page can't generate a full-packed , easy-to-use player for me.

Create this for new DPlayer users like me. Let others become easier to use DPlayer , just by a simple link.
