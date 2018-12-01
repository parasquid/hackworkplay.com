---
title: Fixing the Throttling Issue on the Lenovo T480
date: 2018-08-18
tags: ["hack", "thinkpad", "t480", "lenovo"]
image: https://res.cloudinary.com/psqd/image/upload/q_auto:best/v1543672176/2018-08-18_23-11-38.resized.png
---
**TLDR;** [DRAFT] My Lenovo T480 never goes beyond 71C, 15w and 2.2MHz. It seems that something is limiting the power output when using GNU/Linux. Fortunately there's a tool you can use to sidestep this limitation and be able to use the full power of the laptop, at the cost of more heat and louder fan spin.
<!--more-->

Investigation here: [https://www.reddit.com/r/thinkpad/comments/870u0a/t480s_linux_throttling_bug/](https://www.reddit.com/r/thinkpad/comments/870u0a/t480s_linux_throttling_bug/)
![s-tui tool](2018-08-18-fixing-the-throttling-issue-on-the-lenovo-t480.html/2018-08-18_23-11-38.resized.png)
*The [s-tui](https://github.com/amanusk/s-tui) tool showing the default thermal limits of the laptop*

Fix it with this tool: [https://github.com/erpalma/lenovo-throttling-fix](https://github.com/erpalma/lenovo-throttling-fix)

