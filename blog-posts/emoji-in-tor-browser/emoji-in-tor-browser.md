Typically the browser displays a tofu character, and nothing is useful anymore.

Since TorBrowser is based on Firefox, we can use a font specifically designed for firefox usage, and embed it in the page.

In docusaursus, think set up fonts in customcss page somehow

Steps to get it on the page:

1. Grab the firefox font from https://github.com/mozilla/fxemoji

Find an emoji that is different in chrome to the fxemoji, so can know the page is loading it correctly.

Twitter color emoji can be used, but this is very heavy to download Can bang that down to a 256kb woff2 font file using: https://onlinefontconverter.com/

Use stylesheet:

```css
@font-face {
  font-family: 'Firefox Emoji';
  src: url('FirefoxEmoji.woff2') format('woff2');
  font-weight: normal;
  font-style: normal;
  font-display: swap;
}
```

Tools used: https://wakamaifondue.com/ Extraordinarily helpful too to see fonts working in Tor before going thru deployment.

If you want to make the size smaller, use these tools to punch out a subset of the fonts:

Links to terminal to see it in action.
