# bootstrap6-tour

This is a modern Bootstrap 6 tour. Requires Bootstrap 6 JS + CSS. Originally part of [uproot-examples](https://github.com/mrpg/uproot-examples).

A Bootstrap 5 tour is available [here](https://raw.githubusercontent.com/mrpg/uproot-examples/74f20559681d18a3a5f2524b763e45b4176e21c7/bootstrap_elements/_static/tour.js) ([CSS](https://raw.githubusercontent.com/mrpg/uproot-examples/74f20559681d18a3a5f2524b763e45b4176e21c7/bootstrap_elements/_static/tour.css)).

## Usage

Load Bootstrap 6 CSS and JS, then include `tour.css` and `tour.js`. See [example.html](example.html) for a complete example using a CDN.

```html
<link rel="stylesheet" href="tour.css">
<script src="tour.js"></script>
<script>
    Tour.start([
        {
            target: "#my-element",
            title: "Welcome",
            content: "An explanation of this element.",
            placement: "bottom",
        },
    ]);
</script>
```

Call `Tour.start(steps)` after the target elements exist. Each step has a CSS selector (`target`), `title`, and plain-text `content`. Optional `placement` is `top`, `right`, `bottom`, or `left`; the tour chooses another side if needed. Missing or hidden targets are skipped.

Use Back/Next or the arrow keys to navigate. Done, Escape, the close button, or a click outside the spotlight ends the tour. Call `Tour.end()` to end it from JavaScript. The rest of the page is inert while the tour runs.

## License

0BSD
