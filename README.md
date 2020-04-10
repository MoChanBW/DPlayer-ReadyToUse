Eng ver | [中文文档](/README_zh.md)
<h1 align="center">DPlayer-Ready to Use</h1>

> Easy to use DPlayer with single URL .

 [![MIT license](https://img.shields.io/github/license/MoChanBW/DPlayer-prepacked)](https://github.com/MoChanBW/DPlayer-prepacked/blob/master/LICENSE)

## Introduction

* Pack [DPlayer](https://github.com/MoePlayer/DPlayer) into single HTML file.

* Using single URL to access DPlayer.

* Using DPlayer in Markdown easily.

## Options

You can custom your player instance by those variables.

> Example Link: https://example.com/DPlayer/?[Name1]=[value1]&[Name2]=[value2] etc.
>
> DEMO : https://dplayer.mochanbw.cn/

|    Name    |          Default           |                                             Description                                              |
|:----------:|:--------------------------:|:----------------------------------------------------------------------------------------------------:|
|  autoplay  |           false            |                                    video autoplay , values: 1 , 0                                    |
|    live    |           false            |      enable live mode, values: 1 , 0. Also see [#live](https://dplayer.js.org/guide.html#live)       |
|   picurl   |   see [#defaultPicurl]()   |                                             video poster                                             |
| playerlogo |      Wait for update       |                                 showing logo in the top left corner                                  |
|   suburl   | 'asset/demoSubtitle_*.vtt' |                                                                                                      |
|  thumburl  |            true            | video thumbnails, generated by [DPlayer-thumbnails](https://github.com/MoePlayer/DPlayer-thumbnails) |
|  vidtype   |           'auto'           |         values: auto , hls , flv , dash , normal , <b>webtorrent</b>*(Need base64 encoded)*          |
|   vidurl   |   see [#defaultVicurl]()   |                                                                                                      |
|  webicon   |      Wait for update       |                                                                                                      |
|  webtitle  |         'DPlayer'          |                                                                                                      |

