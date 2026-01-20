# Audio-Slideshow Extension For Quarto

Adds the option to add/record audio playback to each slide of the presentation. This project ports @rajgoel's [reveal.js](https://github.com/hakimel/reveal.js) [audio-slideshow](https://github.com/rajgoel/reveal.js-plugins/tree/master/audio-slideshow) plugin to [Quarto](https://quarto.org/). Credit goes to [Asvin Goel](https://github.com/rajgoel) for the original plugin.

## Installing

``` bash
quarto add kapsner/audio-slideshow
```

This will install the extension under the `_extensions` subdirectory. If you're using version control, you will want to check in this directory.

## Using

A detailed description of the plugin and its options is given [here](https://github.com/rajgoel/reveal.js-plugins/tree/master/audio-slideshow).

In short:

-  add the plugin to the yaml-header of the qmd file:

```yaml
---
title: "audio-slideshow Example"
format:
  revealjs: default
revealjs-plugins:
  - audio-slideshow
---
```

-   render your project
-   press the key `y` to start the narrative recording - a red circle appears in the upper right corner of the slideshow, indicating that the recorder is running
-   press the key `z` to download the recorded audio in a zip-file
-   extract the downloaded zip-file next to the *html*-file containing the *reveal.js* presentation and rename the folder to `audio/`
-   press the key `a` to toggle the recorded audio playback

## Example

Here is the source code for a minimal example: [example.qmd](example.qmd).
