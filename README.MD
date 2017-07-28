vue-video-background
----
[![npm version](https://badge.fury.io/js/vue-video-background.svg)](https://badge.fury.io/js/vue-video-background)

A Vue component for a full width video background.

This package is in active development. Feel free to contribute.
If you have any problems please open an issue on Github.

## Usage

1. Install via npm

``` npm install --save vue-video-background ```

2. Import the component

``` import VueVideoBackground from 'vue-video-background' ```

3. Use the component

You must at least give the videoSrc-prop.

``` <vue-video-background videoSrcWebm="path/to/your/video/file.webm"></vue-video-background> ```

Source file can be .webm or mp4 or specify both types for greater browser support. Webm will always be used first.


## Settings

Option | Type | Default | Description
------ | ---- | ------- | -----------
videoSrcWebm | string | '' | The path to your .webm video source.
videoSrcMp4 | string | '' | The path to your .mp4 video source.
poster | string | '' | Path to preview image. Will be replaced by video once it loads.
textOverlay | boolean | false | Whether to show a text overlay or not.
textHeadline | string | '' | The Headline for your text overlay. Will be in h1-tags.
textSubtitle | string | '' | The Subtitle for your text overlay. Will be in h2-tags.
textBody | string | '' | The text for your text overlay. Will be in p-tags.
