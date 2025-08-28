---
layout: page
title: "WhatTheFund"
description: "A webapp that attempts to lower the entry into investing in ETF's using LLMS to explain concepts and investment opportunities"
technologies: ["LLM's", "python", "Ollama", "React"]
featured: true
date: 2025-06-08
---

## What The Fuck is WhatTheFund

WhatTheFund is a webapp, that uses LLM's to give an analysis of ETF's that are fetched using the Yahoo Finance api. 
The LLM gets a lot of information available of the api, and tries to evaluate what kind of investment the ETF is, what the expected return is on longterm etc.

![A screenshot of the WTF overview](/assets/pictures/wtf_landing_chopped.png)

Next to this analysis, another LLM, trained for economic and political purposes is used to give more insight into this ETF.
It can help to base actual investment inspiration more on this insight than the analysis.

![A screenshot of the ETF overview](/assets/pictures/wtf_AI_gen_chopped.png)

Another problem that WTF tries to tackle, is the difficulty of entering investing. 
Because investing involves a very uncommon jargon, it's difficult to understand what different things mean, what is good and bad, etc.
That is why I've made the "Ask WTF" button, that appears everytime you select some text. 
This button then opens a chat which explains the part that you just selected, and with which you can chat further about the same or different subjects.

![demonstration of the Ask WTF button](/assets/gifs/wtfund_ask_chopped.gif)

