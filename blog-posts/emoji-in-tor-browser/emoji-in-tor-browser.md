---
published: false
title: 'Emoji in the TOR Browser'
cover_image: 'https://raw.githubusercontent.com/dreamcatcher-tech/dev.to/master/blog-posts/anonymous-coding/assets/dragon.jpg'
description: 'Emoji in the TOR Browser'
tags: infosec, privacy, tor
series:
canonical_url: https://github.com/dreamcatcher-tech/dev.to/blob/master/blog-posts/emoji-in-tor-browser/emoji-in-tor-browser.md
---

The TOR browser has to limit the emoji characters it displays since the range of fonts available varies between computers and can be used to deanonymize a user.

Typically the browser displays a tofu character, and nothing is useful anymore, but since TorBrowser is based on Firefox, we can use a font specifically designed for firefox usage, and embed it in the page.

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

Links to terminal to see it in action.
