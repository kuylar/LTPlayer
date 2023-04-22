# LTPlayer

A video player made for [LightTube](https://github.com/kuylar/lighttube).

## Usage

just import `src/player.js` & `src/player.css` into your HTML file, and then initialize the player with the following
snippet:

```html

<script>
	const player = new Player("video", {
		author: {
			icon: "URL of the author icon",
			title: "Name of the video author",
			href: "Link to the author's website"
		},
		title: "Title of the video",
		buttons: {
			// Icons for the control buttons. Accepts HTML.
			// It's recommended to use SVG icons.
			play: '▶',
			pause: '⏸',
			volumeMute: '🔇',
			volumeLow: '🔈',
			volumeMedium: '🔉',
			volumeHigh: '🔊',
			settings: '⚙',
			fullscreen: '🔳',
			minimize: '🔲'
		}
	});
</script>
```

## Styling

You can use CSS variables to style parts of the player.

| CSS Variable                | Description                                   | Default value                               |
|:----------------------------|:----------------------------------------------|:--------------------------------------------|
| ltp-font                    | Font used by the title, timestamp, menus etc. | `"sans-serif"`                              |
| ltp-title-height            | Height of the title element                   | `60px`                                      |
| ltp-top-gradient            | Top gradient of the player.                   | `linear-gradient(to bottom, #0005, #0000)`  |
| ltp-top-gradient-height     | Height of the top gradient.                   | `100px`                                     |
| ltp-controls-height         | Height of the controls row.                   | `40px`                                      |
| ltp-bottom-gradient         | Bottom gradient of the player.                | `linear-gradient(to top, #0005, #0000)`     |
| ltp-bottom-gradient-height  | Height of the bottom gradient.                | `100px`                                     |
| ltp-progress-bar-background | Video playback progress bar background.       | `rgba(255, 255, 255, .2)`                   |
| ltp-progress-bar-buffered   | Video playback buffered bar color.            | `rgba(255, 255, 255, .4)`                   |
| ltp-progress-bar-hover      | Video playback hover bar color.               | `rgba(255, 255, 255, .5)`                   |
| ltp-progress-bar-played     | Video playback played bar color.              | `#F00`                                      |
| ltp-volume-bar-background   | Volume bar background.                        | `rgba(255, 255, 255, .2)`                   |
| ltp-volume-bar-color        | Volume bar color.                             | `#fff`                                      |
| ltp-menu-background         | Menu background.                              | `rgba(28, 28, 28, .9)`                      |
| ltp-menu-hover              | Menu item hover color.                        | `rgba(72, 72, 72, .9)`                      |
| ltp-menu-text               | Menu item text color.                         | `#fff                                     ` |
