# jspsych_smartphone_css
CSS to run [jsPsych](https://www.jspsych.org/v8/) on smartphones
You can view [the demonstration](https://psycho.hes.kyushu-u.ac.jp/~kurokid/image_rating/demo.html). Please use a smartphone.

# The Simplest Method

Just add the following line to the header section.

```html
<meta name="viewport" content="width=device-width,initial-scale=1.0">
```

# More to your liking

This repository provides a sample CSS (`smartphone.css`). Edit this file as you like, and load it in the same way as `jspsych.css`. Note that you need to include the `jspsych.css` before the `smartphone.css`, and the `smartphone.css` doesn't affect the appearance on PC.

```html
<link rel="stylesheet" href="jspsych.css"></link>
<link rel="stylesheet" href="smartphone.css"></link>
```

# Limitations

- A width of 480 pixels or less is considered to be a smartphone. You can change the size freely.
- The CSS file does not enable keyboard input on smartphones.
- The `scale_width` property (e.g., [survey-likert](https://www.jspsych.org/v8/plugins/survey-likert/)) and `slider_width` property (e.g., [html-slider-response](https://www.jspsych.org/v8/plugins/html-slider-response/)) are overwritten by the `smartphone.css`.
- Some CSS properties (e.g., The font size of the prompt in the survey-likert plugin) need to be given a higher priority by specifying `!important`.
- [The free-sort plugin](https://www.jspsych.org/v8/plugins/free-sort/) is not supported.
