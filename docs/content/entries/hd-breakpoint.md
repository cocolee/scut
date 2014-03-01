---
name: hd_breakpoint
type: mixin only
use-name: scut-hd-bp
categories:
  - general
args:
  - variable: $ratio
    default: 1.3
    comment: A *minimum* resolution value.
references:
  - description: The involved Github discussion that resulted in HTML5 Boilerplate's HiDPI breakpoint
    url: https://github.com/h5bp/html5-boilerplate/issues/1127
  - description: Matt Thomas's post about Wordpress's HiDPI breakpoint (implemented in WordPress core 3.5)
    url: http://mattnt.com/2012/11/18/making-sense-of-hidpi-media-queries/
example:
  html: |
    <p class="eg-hd-bp">If you are using a retina screen, this paragraph's background will be blue &mdash; otherwise, a sad low-definition gray.</p>
---

Write effective resolution-based `@media`-queries, without trying too hard.

This mixin uses `-o-min-device-pixel-ratio`, `-webkit-min-device-pixel-ratio`, and `min-resolution`. If you're curious about the choices, read the References below.