<h1 align="center">
Animated SVG clock
</h1>

<p align="center">
<a href="https://tomchen.github.io/animated-svg-clock/clock.svg" title="Click to view the Clock with current time set">
<img src="https://github.com/tomchen/animated-svg-clock/raw/master/clock.svg" alt="Clock"><br>
Click the clock to show a github.io-hosted SVG file where JavaScript is executed to show your current time
</a>
</p>

## Technical details

* CSS-based animation
* Use JavaScript to set the current time
* [![W3C Validation](https://img.shields.io/w3c-validation/default?label=W3C%20SVG%201.1&preset=HTML%2C%20SVG%201.1%2C%20MathML%203.0&targetUrl=https%3A%2F%2Fvalidator.w3.org%2F)](https://validator.w3.org/check?uri=https%3A%2F%2Fraw.githubusercontent.com%2Ftomchen%2Fanimated-svg-clock%2Fmaster%2Fclock.svg&charset=%28detect+automatically%29&doctype=Inline&group=0)

## GitHub usage

JavaScript code of an SVG in `<img>` will not be executed, the [SMIL](https://developer.mozilla.org/en-US/docs/Web/SVG/SVG_animation_with_SMIL) or CSS-based animation is fine, therefore, **what you see on GitHub README.md page is an animated clock starting from 00:00**, it basically counts the time you have stayed on the page.

Even if you open the GitHub.com-hosted (not GitHub.io) raw SVG file ([here it is](https://raw.githubusercontent.com/tomchen/animated-svg-clock/master/clock.svg)) directly in your browser, the JavaScript code will still not be executed due to "[Content Security Policy](https://developer.mozilla.org/en-US/docs/Web/HTTP/CSP): sandbox" header.

In order to execute the JavaScript code and correctly show the current time, you can:

* open a USERNAME.github.io-hosted SVG image ([here is one](https://tomchen.github.io/animated-svg-clock/clock.svg)) directly in your browser
* or download the SVG file, then open it directly in your browser
* or embed it directly (not via `<img>`) in your website, in USERNAME.github.io or any website that does not have strict Content Security Policy header and does not sanitize custom JavaScript code in SVG

Use it (Markdown, can't set width and height):

```markdown
![Clock](https://tomchen.github.io/animated-svg-clock/clock.svg "Clock")
```

Use it (HTML, with width and height set):

```html
<img src="https://tomchen.github.io/animated-svg-clock/clock.svg" alt="Clock" title="Clock" height="200px" width="200px">
```

## Design

Yes it's highly similar to a [Swiss railway clock](https://en.wikipedia.org/wiki/Swiss_railway_clock) whose design [IS COPYRIGHTED](https://www.businessinsider.fr/us/apple-paid-21-million-for-swiss-railways-clock-2012-11).

## Vue3 version

Copy the `AnimatedClock.vue`to your Vue components folder.

And include it in your Vue application somewhere with the following code:

```vue
<script setup>
import AnimatedClock from "@/components/AnimatedClock.vue";
</script>
<template>
  <AnimatedClock />
</template>
```


## Credits

By Tom Chen

Inspired by SVG animation: by HackaLittleBit (https://commons.wikimedia.org/wiki/File:Swiss_railway_clock_1.svg), CC-by-sa 4.0, whose original SVG is: by Jahoe (https://commons.wikimedia.org/wiki/File:Swiss_railway_clock.svg), CC-by-sa 3.0 & GFDL

(The current SVG code has significate code change comparing to HackaLittleBit's work, and is using the permissive MIT license)

## License

MIT license for the code, but Swiss railway clock **DESIGN IS COPYRIGHTED**.
