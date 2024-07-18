---
layout: post
tags: devlog idle_garden
title: "Devlog: Tooltips Implementation in Idle Garden 🌱"
---

![Idle Garden Tooltips](/assets/Idle_Garden_0.10_tooltips.gif){:style="display:block; margin-left:auto; margin-right:auto"}

Today I completed work on version 0.10 of Idle Garden, this version introduces tooltips for the buttons on the sidebar. Here's a breakdown of the implementation process:

### Initial Approach
At first, I tried generating new labels based on the mouse's x, y coordinates. However, having the tips move with the mouse felt a bit chaotic. So, I decided to pin them to a set location based on each button's coordinates.

### Making Labels Legible
The next challenge was ensuring the labels were readable. DragonRuby's label methods don't include background colors, so I created new solid primitives to sit behind the labels. But rendering these solids above other items in the stack, especially the garden background images, turned out to be tricky. In the end, I chose to display the tooltips below all other information labels in the sidebar. This solution actually looks cleaner and avoids obscuring other display information.

### Handling Long Strings
The final hurdle was dealing with long strings. The label primitives don't support text wrapping by default. The docs suggest using a mapping function to cut the text at specific intervals and generate labels from the split content. While this could work, I wanted more control over the label messages. Instead, I updated the JSON file containing the tooltips, manually split the strings where I wanted new lines, and contained them in an array. The `hover?` method now calls `for_each` on the strings and generates a new label for each substring, placing subsequent substrings 20 pixels below the preceding one.

I still intend to work on the actual design but from a functional perspective I pretty pleased with this solution. Stay tuned for more updates!

Happy gardening! 🌼
