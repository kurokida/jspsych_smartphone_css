# jspsych_smartphone_css
CSS to run [jsPsych](https://www.jspsych.org/v8/) on smartphones

# The Simplest Method

Just add the following line to the header section.

```html
<meta name="viewport" content="width=device-width,initial-scale=1.0">
```

# More to your liking

This repository provides a sample CSS (smartphone.css). Edit this file as you like, and load it in the same way as jspsych.css.

```html
<link rel="stylesheet" href="smartphone.css"></link>
```

# Limitations

- A width of 480 pixels or less is considered to be a smartphone. You can change the size freely.
- The CSS file does not enable keyboard input on smartphones.
- It is not possible to specify `scale_width` and `slider_width` for each device. Therefore, it is necessary to specify the most suitable size for all devices.
- Modifying the prompt text in the questions of [the survey-likert plugin](https://www.jspsych.org/v8/plugins/survey-likert/) is a little complicated. Sample files are included in this repository.
- [The free-sort plugin](https://www.jspsych.org/v8/plugins/free-sort/) is not supported.
