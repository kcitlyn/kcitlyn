<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->
<div align="center">

<!-- Banner height trimmed 180 -> 150: it's forced to width:100%, so on GitHub's
     ~1012px column it scales up ~19% and the wave's soft bottom edge left an
     obvious gap under it. All-lowercase to match the terminal on the site. -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:ffd6e8,50:ffb3d1,100:f9a8d4&height=150&section=header&text=hi,%20i'm%20kaitlyn%20✿&fontSize=42&fontColor=4a2540&fontAlignY=36&desc=ece%20@%20ut%20austin%20·%20prev.%20swe%20intern%20@%20aws&descSize=16&descAlignY=60&descAlign=50" width="100%" />

<!-- The typing SVG is back, now with one fixed line instead of a rotation. It's
     an image, so the words themselves can't be links — hence the <a> wrapper
     (whole line → the site) and the badges below, which keep email reachable in
     real clickable form. Height is a tight 45 to keep the stacked-image margin
     under it small. -->
<a href="https://kaitlynchen.dev"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=19&pause=1200&color=FFB3D1&center=true&vCenter=true&width=650&height=45&lines=want%20to%20know%20more%3F%20%E2%86%92%20kaitlynchen.dev%20%20%C2%B7%20%20or%20just%20say%20hi%20%E2%9C%BF" alt="want to know more? → kaitlynchen.dev · or just say hi ✿" /></a>

[![Portfolio](https://img.shields.io/badge/✿_my_portfolio-kaitlynchen.dev-FFB3D1?style=for-the-badge&logoColor=4A2540&labelColor=FFD6E8)](https://kaitlynchen.dev)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-F9A8D4?style=for-the-badge&logo=linkedin&logoColor=4A2540&labelColor=FFD6E8)](https://www.linkedin.com/in/kaitlynychen)
[![Email](https://img.shields.io/badge/say_hi-FFC1DD?style=for-the-badge&logo=gmail&logoColor=4A2540&labelColor=FFD6E8)](mailto:kcitlynychen@gmail.com)

<sub>made with 💗 by kaitlyn — hand-written markdown, no generator</sub>

</div>

<!-- No stats/highlights strip here on purpose: it restated the project cards
     below almost verbatim, and a bare metric with a three-word caption reads as
     jargon to anyone who hasn't already seen the resume. The projects section
     makes the same points once, with the context that makes them land. -->

<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->

## ✿ about me

```python
kaitlyn = {
    "school":    "BS Electrical & Computer Engineering, UT Austin '28",
    "focus":     "Computer Architecture & Embedded Systems",
    "prev":      "SWE Intern @ AWS — GenAI Developer Tools",
    "lives_in":  "Austin, TX (school year)  ·  Houston, TX (home)",
    "works_on":  ["agentic AI tooling", "embedded systems", "edge ML"],
    "ask_me_about": "the last concert I went to (there are many)",
    "highlight": "1st place at Amazon's internal hackathon — 190+ engineers, "
                 "judged by a panel of L8 senior leaders 🏆",
}
```

I work in the overlap between **embedded systems** and **machine learning** — close
enough to the hardware to care about clock cycles, close enough to the models to
care about what they get wrong. I like problems where the answer has to survive
contact with real hardware, and I tend to chase an idea until it actually *works*.

Being a **first-gen student** taught me to reverse-engineer systems nobody
explained to me, which is conveniently most of engineering.

<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->

## ✿ things I've built

<!-- Every project here follows the same shape on purpose: heading → one or two
     sentences of what it is → the single number that proves it → tags + link.
     The old version opened with nested "matching engine / what I owned" bullet
     lists, which is résumé density in a place people are skimming — nobody
     reads twelve bullets on a profile page. The engineering detail didn't get
     deleted, it moved to the site, which is where someone who wants it goes. -->

> A sentence each — the **full write-ups** live on **[kaitlynchen.dev →](https://kaitlynchen.dev)**

<br/>

### 🥇 Ctrl+Meet &nbsp;·&nbsp; [`repo →`](https://github.com/kcitlyn/ctrl-meet)

A cross-team matchmaking platform for interns who get flown to a new city and
seated on heads-down teams. A 16-question survey feeds a recommender that
auto-weights each question by how much it actually distinguishes people, then
re-ranks for variety so your matches aren't five copies of you. Shipped on real
AWS behind SSO, not localhost.

**🏆 Grand prize — the whole hackathon, out of 190+ engineers**, picked by a
cohort-wide peer vote and then a panel of Amazon L8 senior leaders.

`React` `Lambda` `DynamoDB` `Bedrock` `Titan` `API Gateway` `CDK` `RAG` `Vitest`

<br/>

### 🤖 Agent tooling at AWS &nbsp;·&nbsp; *SWE intern, GenAI Developer Tools*

LLM agents are normally stuck with whatever tools they booted with. I built a
proxy that runs child MCP servers as live subprocesses, so an agent can install
a capability and use it **mid-session with no restart** — then wired it to a
~4,000-server enterprise registry it can search on its own.

**3 services, ~200 tests, and warm tool lookups under 10ms** (down from ~2s
cold), hardened against prompt injection and tool poisoning.

`TypeScript` `Java` `MCP` `Lambda` `DynamoDB` `Bedrock` `CDK` `CloudWatch`

<br/>

### 🚗 Texas EcoCar &nbsp;·&nbsp; *ML steering controller for an autonomous vehicle*

Replaced the hand-tuned PID steering controller on UT's autonomous vehicle with
a Gaussian Process model — no manual calibration, same tracking quality. The
nice part: the GP reports its own uncertainty, so the car can tell when it's
outside what it was trained on and fall back before that becomes a problem.

**0.23 m RMSE lane tracking**, trained on a 678,000-point system-ID pipeline.

`C/C++` `MATLAB/Simulink` `Python` `Controls`

<br/>

### 🎙️ PolyScribe &nbsp;·&nbsp; [`repo →`](https://github.com/kcitlyn/PolyScribe_Desktop)

<!-- Live badges, not hardcoded numbers: shields.io reads the GitHub API on every
     page load, so these can't quietly go stale the way "⭐13" would the moment
     someone else stars it. -->
[![Stars](https://img.shields.io/github/stars/kcitlyn/PolyScribe_Desktop?style=flat-square&label=stars&color=FFB3D1&labelColor=FFD6E8)](https://github.com/kcitlyn/PolyScribe_Desktop/stargazers)
[![Forks](https://img.shields.io/github/forks/kcitlyn/PolyScribe_Desktop?style=flat-square&label=forks&color=F9A8D4&labelColor=FFD6E8)](https://github.com/kcitlyn/PolyScribe_Desktop/forks)

Speech-to-text and translation across **20+ languages**, running entirely on
your own machine — no cloud, no API keys, nothing leaving the device.

**People I've never met found it, starred it, forked it, and started filing
feature requests.** Nobody asked them to — still the most fun feedback I've
gotten.

`Python` `Vosk` `Argos` `pyttsx3`

<br/>

### 🩺 edgedoctor &nbsp;·&nbsp; [`repo →`](https://github.com/kcitlyn/edgedoctor) &nbsp;*(in progress)*

Tells you why your model got slow or broke once you put it on real edge
hardware — quantization mismatches, unsupported ops, memory pressure — instead
of leaving you to guess.

`Python` `Edge AI` `ML Tooling`

<br/>

### 🚄 Texas Guadaloop &nbsp;·&nbsp; *hyperloop pod firmware*

Real-time Hall-effect speed sensing on **STM32**, using ADC with DMA circular
buffering so samples never get dropped. I also wrote the pod-wide embedded
architecture reference — 9 distributed nodes, CAN routing, LoRa link to the
ground station — which became the doc the whole team wired against.

`C` `STM32` `CAN` `ADC/DMA` `UART`

<br/>

### and a couple more

| | |
|---|---|
| 👤 **[TrainYourFace](https://github.com/kcitlyn/TrainYourFace)** | Real-time multi-face recognition that runs fully offline, with a tunable tradeoff between false matches and missed ones. `Python` `OpenCV` `dlib` |
| 🌌 **Astrarium** · *HackTX 2025* | LLM backend that validates every model response and falls back gracefully, so a flaky model never takes the app down. `FastAPI` `PostgreSQL` `Next.js` |

<div align="center">

<br/>

### ✿ there's more on the site ✿

Every project above, written up properly — plus an interactive circuit-board
background I probably spent too long on.

[![Portfolio](https://img.shields.io/badge/✿_read_the_full_thing-kaitlynchen.dev-FFB3D1?style=for-the-badge&logoColor=4A2540&labelColor=FFD6E8)](https://kaitlynchen.dev)

</div>

<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->

## ✿ my toolbox

<div align="center">

**languages**

<img src="https://skillicons.dev/icons?i=py,c,cpp,ts,js,matlab,bash,latex&theme=light" />

`C/C++` · `Python` · `TypeScript/JavaScript` · `MATLAB` · `Assembly (ARM Cortex-M0, LC-3)` · `LaTeX`

**AI / agentic**

`MCP (Model Context Protocol)` · `LLM agents` · `RAG` · `prompt engineering` · `evals & benchmarking` · `structured-output validation` · `prompt-injection defense`

**embedded & hardware**

<img src="https://skillicons.dev/icons?i=arduino,raspberrypi&theme=light" />

`STM32` · `ARM Cortex-M0` · `CAN bus` · `I2C/SPI/UART` · `ADC/DMA` · `real-time systems` · `FSM design` · `timers/interrupts` · `PCB layout` · `KiCad` · `LTSpice` · `datasheet bring-up` · `logic analyzer` · `oscilloscope`

**ML / perception**

`OpenCV` · `Gaussian Process regression` · `system identification` · `real-time video inference` · `dlib` · `ResNet` · `Vosk (STT)` · `Argos (NMT)`

**systems, web & cloud**

<img src="https://skillicons.dev/icons?i=react,nextjs,tailwind,fastapi,postgres,aws,docker,linux,git,cmake&theme=light" />

`Linux` · `GDB` · `Valgrind` · `concurrency/multithreading` · `REST APIs` · `AWS Lambda` · `DynamoDB` · `CloudWatch` · `CDK`

</div>

<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->

## ✿ recognition

| | |
|---|---|
| 🏆 | **1st Place — Amazon Internal Hackathon** · winner among 190+ engineers |
| 🌸 | **NCWIT Aspirations in Computing** · National Honorable Mention **&** Houston Affiliate Winner |
| 🎓 | **Engineering Honors** + **Engineering Honors Scholarship** · UT Austin Cockrell School |
| ✨ | **National First-Gen Recognition** |

<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->

## ✿ currently

- 🌱 **learning** — how far I can push real models onto small hardware before they stop being useful
- 💌 **looking for** — SWE / ML / embedded / edge-AI internships
- 🎧 **outside of code** — hiking, sudoku, and a steady rotation of Raspberry Pi projects

<br/>

<div align="center">

### ✿ let's build something ✿

I'm always happy to talk about embedded systems, edge ML, or agentic AI —
or to hear about a project you're excited about.

[![Email](https://img.shields.io/badge/kcitlynychen@gmail.com-FFD6E8?style=for-the-badge&logo=gmail&logoColor=4A2540)](mailto:kcitlynychen@gmail.com)
[![Portfolio](https://img.shields.io/badge/kaitlynchen.dev-FFB3D1?style=for-the-badge&logo=vercel&logoColor=4A2540)](https://kaitlynchen.dev)
[![LinkedIn](https://img.shields.io/badge/kaitlynychen-F9A8D4?style=for-the-badge&logo=linkedin&logoColor=4A2540)](https://www.linkedin.com/in/kaitlynychen)

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:f9a8d4,50:ffb3d1,100:ffd6e8&height=120&section=footer&text=thanks%20for%20scrolling%20✿&fontSize=20&fontColor=4a2540&fontAlignY=72" width="100%" />

</div>
