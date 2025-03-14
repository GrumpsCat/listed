---
author: Hugo Authors
title: What is the biological basis for dreams and nightmares?
date: 2021-07-10T07:00:00+00:00
description: A brief guide to setup KaTeX
math: true
draft: true
---
## What is sleep?

Sleep is "a reversible behavioral state of perceptual disengagement from and unresponsiveness to the environment." (Carskadon 2005). 

Physiologically,  sleep can be broken down into two states, rapid eye movement (REM) and non-REM (NREM) states. 

NREM can be thought of as having an inactive brain in a moveable body. NREM has four stages (1, 2, 3 and 4) where arousal is lowest in 1 and highest in 4. 

[Carskadon, Mary A., and William C. Dement. "Normal human sleep: an overview." _Principles and practice of sleep medicine_4.1 (2005): 13-23.](https://git.auror.ar/maltalef/tesina-2021/raw/commit/f2792d0b3f0a85574de5d24a8521bccc2c44b168/material-de-lectura/carskadon2011.pdf)

## What is the physiology of sleep?

## What defines a dream and nightmare?

Mathematical notation in a Hugo project can be enabled by using third party JavaScript libraries.
<!--more-->

In this example we will be using [KaTeX](https://katex.org/)

* Create a partial under `/layouts/partials/math.html`
* Within this partial reference the [Auto-render Extension](https://katex.org/docs/autorender.html) or host these scripts locally.
* Include the partial in your templates like so:

```bash
{{ if or .Params.math .Site.Params.math }}
{{ partial "math.html" . }}
{{ end }}
```

* To enable KaTex globally set the parameter `math` to `true` in a project's configuration
* To enable KaTex on a per page basis include the parameter `math: true` in content files

**Note:** Use the online reference of [Supported TeX Functions](https://katex.org/docs/supported.html)

{{< math.inline >}}
{{ if or .Page.Params.math .Site.Params.math }}
<!-- KaTeX -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@0.11.1/dist/katex.min.css" integrity="sha384-zB1R0rpPzHqg7Kpt0Aljp8JPLqbXI3bhnPWROx27a9N0Ll6ZP/+DiW/UqRcLbRjq" crossorigin="anonymous">
<script defer src="https://cdn.jsdelivr.net/npm/katex@0.11.1/dist/katex.min.js" integrity="sha384-y23I5Q6l+B6vatafAwxRu/0oK/79VlbSz7Q9aiSZUvyWYIYsd+qj+o24G5ZU2zJz" crossorigin="anonymous"></script>
<script defer src="https://cdn.jsdelivr.net/npm/katex@0.11.1/dist/contrib/auto-render.min.js" integrity="sha384-kWPLUVMOks5AQFrykwIup5lo0m3iMkkHrD0uJ4H5cjeGihAutqP0yW0J6dpFiVkI" crossorigin="anonymous" onload="renderMathInElement(document.body);"></script>
{{ end }}
{{</ math.inline >}}

### Examples

{{< math.inline >}}
<p>
Inline math: (\\varphi = \\dfrac{1+\\sqrt5}{2}= 1.6180339887…)
</p>
{{</ math.inline >}}

Block math:
$$
\\varphi = 1+\\frac{1} {1+\\frac{1} {1+\\frac{1} {1+\\cdots} } }
$$
