---
layout: post
tags: devlog idle_garden
title: "Devlog: Debt in Idle Garden 🌱"
---

![Idle Garden 0.13](/assets/idle_garden_0.13_debt.png){:style="display:block; margin-left:auto; margin-right:auto"}

Today I've released version 0.12 of [Idle Garden](https://jalamb5.itch.io/idle-garden). Here’s what’s new in this update:

### Debt
Previously, players could find themselves stuck with no seeds, cash, or harvestable plants, forcing a game reset. Now, if you get into this situation, you’ll be given 5 seeds and incur a debt of 30. This debt is slightly more expensive than buying 5 seeds outright, so try to avoid this scenario if you can.

### Automator Cooldowns
I’ve tweaked the cooldowns for auto planters, harvesters, and sellers. Planters will now run more frequently, sellers less frequently, while harvesters continue at their previous pace. This should help balance the automation process a bit better.

### Alerts
If you’ve read previous devlogs, you’ll know I recently [introduced tooltips](https://blog.justinlamb.org/2024/08/03/Devlog-Levels-Idle-Garden/) for the sidebar buttons. Today, these tooltips have been migrated to an all-new Alerts system. For players, this won’t look any different, but it allows me to display info in the sidebar more easily moving forward. The new debt system is the first use case for this, a brief message will now pop up to let players know they've incurred a debt.

That’s all for this update! Stay tuned for more updates.

Happy gardening! 🌼
