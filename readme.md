# Binary Christmas Tree

This repo hosts a single-page holiday greeting that renders a rotating Christmas tree built from **0**s and **1**s.

## How it works
- `index.html` contains the entire page (HTML, CSS, and JavaScript) so it can be deployed on GitHub Pages or any static host without a build step.
- The page centers a `<pre>` element inside a `.scene` container with CSS perspective and applies a `rotateY` animation to create the spinning effect.
- JavaScript generates the tree on the fly: each row mirrors randomly generated binary digits to keep the silhouette symmetric, while `span.digit` elements colorize foliage (`0`), multicolor fairy lights (`1`), and the trunk.
- A timer refreshes the tree every ~1.8 seconds, so the lights twinkle as the tree spins.
