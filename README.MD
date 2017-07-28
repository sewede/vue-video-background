vue-video-background
----

A Vue component for a full width video background.

## Usage

1. Install via npm

``` npm install --save vue-video-background ```

2. Import the component

``` import VueVideoBackground from 'vue-video-background' ```

3. Use the component

You must at least give the videoSrc-prop.

``` <vue-video-background videoSrc="path/to/your/video/file.webm"></vue-video-background> ```


## Settings

Option | Type | Default | Description
------ | ---- | ------- | -----------
videoSrc | string | '' | The path to your video source.
textOverlay | boolean | false | Whether to show a text overlay or not.
textHeadline | string | '' | The Headline for your text overlay. Will be in h1-tags.
textSubtitle | string | '' | The Subtitle for your text overlay. Will be in h2-tags.
textBody | string | '' | The text for your text overlay. Will be in p-tags.
