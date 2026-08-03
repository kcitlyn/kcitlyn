<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->
<div align="center">

<!-- Banner height trimmed 180 -> 150: it's forced to width:100%, so on GitHub's
     ~1012px column it scales up ~19% and the wave's soft bottom edge left an
     obvious gap under it. All-lowercase to match the terminal on the site. -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:ffd6e8,50:ffb3d1,100:f9a8d4&height=150&section=header&text=hi,%20i'm%20kaitlyn%20✿&fontSize=42&fontColor=4a2540&fontAlignY=36&desc=ece%20@%20ut%20austin%20·%20prev.%20sde%20intern%20@%20aws&descSize=16&descAlignY=60&descAlign=50" width="100%" />

<!-- "currently:" is baked INTO the svg rather than sitting next to it as bold
     markdown. It has to be: GitHub strips author style attributes, so text in
     the page can't be given the SVG's font (Fira Code), its size (18px), or its
     pink. It renders in GitHub's body font at body size in body color, and no
     amount of markup fixes the mismatch or the word-space gap between a text
     node and an inline image. Inside the SVG, one text element draws the whole
     line, so the alignment problem can't exist. Cost: the prefix retypes each
     loop, which is the right trade for it actually matching.

     width MUST clear the longest line or center=true overflows both edges and
     clips the first character. Fira Code is monospace at 0.6em advance, so the
     math is chars x size x 0.6: the internships line is 62 chars x 18 x 0.6 =
     ~670px, which is why 650 cut the "c" off. 720 leaves ~50px of slack. If you
     add a longer line, re-run that multiplication first. -->
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=18&pause=1600&color=FFB3D1&center=true&vCenter=true&width=720&height=40&lines=currently%3A%20open%20to%20summer%202027%20SWE%20%2F%20ML%20%2F%20embedded%20internships;currently%3A%20still%20awake%20because%20the%20bug%20was%20almost%20fixed;currently%3A%20studying%20computer%20architecture%20and%20edge%20ML" alt="currently: open to summer 2027 SWE / ML / embedded internships · still awake because the bug was almost fixed · studying computer architecture and edge ML" />

[![Portfolio](https://img.shields.io/badge/✿_my_portfolio-kaitlynchen.dev-FFB3D1?style=for-the-badge&logoColor=4A2540&labelColor=FFD6E8)](https://kaitlynchen.dev)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-F9A8D4?style=for-the-badge&logo=linkedin&logoColor=4A2540&labelColor=FFD6E8)](https://www.linkedin.com/in/kaitlynychen)
[![Email](https://img.shields.io/badge/say_hi-FFC1DD?style=for-the-badge&logo=gmail&logoColor=4A2540&labelColor=FFD6E8)](mailto:kcitlynychen@gmail.com)

<sub>made with 💗 by kaitlyn · hand-written markdown, no generator</sub>

</div>

<!-- No stats/highlights strip here on purpose: it restated the project cards
     below almost verbatim, and a bare metric with a three-word caption reads as
     jargon to anyone who hasn't already seen the resume. The projects section
     makes the same points once, with the context that makes them land. -->

<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->

## ✿ about me

```python
kaitlyn = {
    "school":    "BS Electrical & Computer Engineering, UT Austin",
    "focus":     "Computer Architecture & Embedded Systems",
    "prev":      "SDE Intern @ AWS · GenAI Developer Tools",
    "lives_in":  "Austin, TX (school year)  ·  Houston, TX (home)",
    "works_on":  ["agentic AI tooling", "embedded systems", "edge ML"],
    "ask_me_about": "the last concert I went to (there are many)",
    "fun_fact":  "1st place at Amazon's internal hackathon: 190+ engineers, "
                 "judged by a panel of L8 senior leaders 🏆",
}
```

I work in the overlap between **embedded systems** and **machine learning**. Close
enough to the hardware to care about clock cycles, close enough to the models to
care about what they get wrong. I like problems where the answer has to survive
contact with real hardware, and I tend to chase an idea until it actually *works*.

Being a **first-gen student** taught me to reverse-engineer systems nobody
explained to me, which is conveniently most of engineering.

<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->

## ✿ things I've built

<!-- One or two lines each, then a link out. This section is a table of contents,
     not the documentation: anyone still reading by the third paragraph was going
     to click through anyway, and anyone who wasn't had already stopped. Full
     write-ups live on the site, engineering detail lives in each repo. -->

> Short version here. **Full write-ups on [kaitlynchen.dev →](https://kaitlynchen.dev)**

<br/>

### 🥇 Ctrl+Meet &nbsp;·&nbsp; [`repo →`](https://github.com/kcitlyn/ctrl-meet)

Cross-team matchmaking for interns flown to a new city and seated on heads-down
teams. A 16-question survey feeds a recommender that weights each question by how
much it actually distinguishes people. Shipped on real AWS behind SSO.

**🏆 We won the whole hackathon, out of 190+ engineers**, judged by a panel of
Amazon L8 senior leaders.

`React` `Lambda` `DynamoDB` `Bedrock` `RAG` `CDK`

<br/>

### 👤 TrainYourFace &nbsp;·&nbsp; [`repo →`](https://github.com/kcitlyn/TrainYourFace)

Face recognition that knows when it's being fooled. A liveness model tells a real
face from a photo or a phone screen, and recognition is gated behind it, so
holding up a picture of me doesn't unlock anything.

**Liveness in 0.44 ms** on a 1.0 MB model, scored with the ISO/IEC 30107-3
metrics the field actually reports.

`Python` `PyTorch` `ONNX Runtime` `CoreML` `Anti-spoofing` `Edge AI`

<br/>

### 🤖 Agent tooling at AWS &nbsp;·&nbsp; *SDE intern, GenAI Developer Tools*

LLM agents are normally stuck with whatever tools they booted with. I built a
proxy that runs child MCP servers as live subprocesses, so an agent can install a
capability and use it **mid-session with no restart**.

**3 services, ~200 tests, warm tool lookups under 10ms**, hardened against
prompt injection and tool poisoning.

`TypeScript` `Java` `MCP` `Lambda` `DynamoDB` `Bedrock` `CDK`

<br/>

### 🚗 Texas EcoCar &nbsp;·&nbsp; *ML steering controller for an autonomous vehicle*

Replaced the hand-tuned PID steering controller on UT's autonomous vehicle with a
Gaussian Process model, which needs no manual calibration and reports its own
uncertainty, so the car can tell when it's outside what it was trained on.

**0.23 m RMSE lane tracking**, trained on a 678,000-point system-ID pipeline.

`C/C++` `MATLAB/Simulink` `Python` `Controls`

<br/>

### 🎙️ PolyScribe &nbsp;·&nbsp; [`repo →`](https://github.com/kcitlyn/PolyScribe_Desktop)

[![Stars](https://img.shields.io/github/stars/kcitlyn/PolyScribe_Desktop?style=flat-square&label=stars&color=FFB3D1&labelColor=FFD6E8)](https://github.com/kcitlyn/PolyScribe_Desktop/stargazers)
[![Forks](https://img.shields.io/github/forks/kcitlyn/PolyScribe_Desktop?style=flat-square&label=forks&color=F9A8D4&labelColor=FFD6E8)](https://github.com/kcitlyn/PolyScribe_Desktop/forks)

Speech-to-text and translation across **20+ languages**, running entirely on your
own machine. No cloud, no API keys, nothing leaving the device.

**Strangers found it, starred it, forked it, and started filing feature
requests.** Still the most fun feedback I've gotten.

`Python` `Vosk` `Argos`

<br/>

### 🩺 edgedoctor &nbsp;·&nbsp; [`repo →`](https://github.com/kcitlyn/edgedoctor) &nbsp;*(in progress)*

Tells you why your model broke or got slow once you put it on real edge hardware,
instead of leaving you to guess.

`Python` `Edge AI` `ML Tooling`

<br/>

### 🌌 Astrarium &nbsp;·&nbsp; *HackTX 2025*

LLM backend that validates every model response and falls back gracefully, so a
flaky model never takes the app down.

`FastAPI` `PostgreSQL` `Next.js`

<br/>

<div align="center">

<br/>

### ✿ there's more on the site ✿

Every project above, written up properly, plus an interactive circuit-board
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

`PyTorch` · `ONNX Runtime` · `CoreML` · `OpenCV` · `INT8 quantization` · `anti-spoofing / PAD` · `Gaussian Process regression` · `system identification` · `real-time video inference` · `Vosk (STT)` · `Argos (NMT)`

**systems, web & cloud**

<img src="https://skillicons.dev/icons?i=react,nextjs,tailwind,fastapi,postgres,aws,docker,linux,git,cmake&theme=light" />

`Linux` · `GDB` · `Valgrind` · `concurrency/multithreading` · `REST APIs` · `AWS Lambda` · `DynamoDB` · `CloudWatch` · `CDK`

</div>

<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->

## ✿ recognition

| | |
|---|---|
| 🏆 | **1st Place, Amazon Internal Hackathon** · winner among 190+ engineers |
| 🌸 | **NCWIT Aspirations in Computing** · National Honorable Mention **&** Houston Affiliate Winner |
| 🎓 | **Engineering Honors** + **Engineering Honors Scholarship** · UT Austin Cockrell School |
| ✨ | **National First-Gen Recognition** |

<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->

## ✿ currently

- 🌱 **learning**: how far I can push real models onto small hardware before they stop being useful
- 💌 **looking for**: SWE / ML / embedded / edge-AI internships
- 🎧 **outside of code**: hiking, sudoku, and a steady rotation of Raspberry Pi projects

<br/>

<div align="center">

### ✿ let's build something ✿

My inbox is open for anything: a role, a project, a question, a cool thing you
made, or just to say hi. I answer everyone.

[![Email](https://img.shields.io/badge/kcitlynychen@gmail.com-FFD6E8?style=for-the-badge&logo=gmail&logoColor=4A2540)](mailto:kcitlynychen@gmail.com)
[![Portfolio](https://img.shields.io/badge/kaitlynchen.dev-FFB3D1?style=for-the-badge&logo=vercel&logoColor=4A2540)](https://kaitlynchen.dev)
[![LinkedIn](https://img.shields.io/badge/kaitlynychen-F9A8D4?style=for-the-badge&logo=linkedin&logoColor=4A2540)](https://www.linkedin.com/in/kaitlynychen)

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:f9a8d4,50:ffb3d1,100:ffd6e8&height=120&section=footer&text=thanks%20for%20scrolling%20✿&fontSize=20&fontColor=4a2540&fontAlignY=72" width="100%" />

</div>
