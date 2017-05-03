[![Build Status](https://travis-ci.org/mpachnis/mp-video.svg?branch=master)](https://travis-ci.org/mpachnis/mp-video) [![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/mpachnis/mp-video)


## &lt;mp-slider&gt;

YouTube, Vimeo and HTML5 video playback web component.


## How it works

Specify the video type you want to embed: `youtube`, `vimeo` or `html-video`,
add the video source you want, for youtube and vimeo you must specify the `video-id`, for `html-video` the `html-video-mp4`, `html-video-ogg` or `html-video-webm`. That's it.
Videos designed to be responsive. Wrap the `<mp-video>` to a div and set the width into that div.


## Demo

[mp-slider docs & demo](https://www.webcomponents.org/element/mpachnis/mp-video)


## Install the component using [Bower](http://bower.io/):

```bash
$ bower install --save mp-video
```

## Usage

1. Import Web Components' polyfill:

```html
<script src="bower_components/webcomponentsjs/webcomponents-lite.js"></script>
```

2. Import Custom Element:

```html
<link rel="import" href="bower_components/mp-video/mp-video.html">
```

3. Start using it!

<!--
```
<custom-element-demo>
    <template>
        <script src="../webcomponentsjs/webcomponents-lite.js"></script>
        <link rel="import" href="mp-video.html">
        <next-code-block></next-code-block>
    </template>
</custom-element-demo>
```
-->

```html
<mp-video youtube
          video-id="8-Zq2KUN6jM"
          video-volume="60"
          video-autoplay="0">
</mp-video>
<mp-video vimeo
          video-id="78323839"
          video-autoplay="0"
          video-volume="0.5">
</mp-video>
<mp-video html-video
          video-controls
          video-preload="auto"
          video-volume="0.5"
          video-thumnail="https://www.html5rocks.com/en/tutorials/video/basics/poster.png"
          html-video-mp4="https://www.html5rocks.com/en/tutorials/video/basics/devstories.mp4"
          html-video-webm="https://www.html5rocks.com/en/tutorials/video/basics/devstories.webm">
</mp-video>
```

## License

MIT License
