<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:ffd6e8,50:ffb3d1,100:f9a8d4&height=180&section=header&text=hi,%20I'm%20Kaitlyn%20✿&fontSize=44&fontColor=4a2540&fontAlignY=34&desc=ECE%20@%20UT%20Austin%20·%20I%20make%20software%20touch%20the%20real%20world&descSize=16&descAlignY=56&descAlign=50" width="100%" />

<a href="https://kaitlynchen.dev">
  <img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=500&size=21&duration=3400&pause=900&color=F9A8D4&center=true&vCenter=true&width=650&lines=ECE+%40+UT+Austin+%C2%B7+prev.+SWE+Intern+%40+AWS;I+build+agent+runtimes+and+STM32+firmware;1st+place+%F0%9F%8F%86+Amazon+hackathon+%C2%B7+190%2B+engineers;close+to+the+metal%2C+curious+about+the+models" alt="what I do" />
</a>

<br/>

[![Portfolio](https://img.shields.io/badge/✿_my_portfolio-kaitlynchen.dev-FFB3D1?style=for-the-badge&logoColor=4A2540&labelColor=FFD6E8)](https://kaitlynchen.dev)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-F9A8D4?style=for-the-badge&logo=linkedin&logoColor=4A2540&labelColor=FFD6E8)](https://www.linkedin.com/in/kaitlynychen)
[![Email](https://img.shields.io/badge/say_hi-FFC1DD?style=for-the-badge&logo=gmail&logoColor=4A2540&labelColor=FFD6E8)](mailto:kcitlynychen@gmail.com)

</div>

<!-- The skim-in-five-seconds strip. Recruiters read this and nothing else, so
     each line has to be a complete claim on its own — a bare number with a
     three-word caption means nothing to someone who hasn't read the rest.
     Left-aligned on purpose: centered sentence-length lines read ragged. -->
🏆 &nbsp; **Won 1st place at Amazon's internal hackathon**, out of 190+ competing engineers

🤖 &nbsp; **Built the agent tooling behind a ~4,000-server enterprise registry** as an SWE intern at AWS — coding agents can now find and run those tools on their own

🚗 &nbsp; **Replaced a car's hand-tuned steering controller with a machine-learning one** on UT's autonomous vehicle team, and it tracked the lane just as well

🎙️ &nbsp; **Shipped an offline transcription tool people actually use** — 20+ languages, open-source, strangers file feature requests

<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->

## ✿ about me

```python
kaitlyn = {
    "prev":      "SWE Intern @ AWS — GenAI Developer Tools",
    "school":    "BS Electrical & Computer Engineering, UT Austin '28",
    "focus":     "Engineering Honors — Computer Architecture & Embedded Systems",
    "lives_in":  "Austin, TX (school year)  ·  Houston, TX (home)",
    "works_on":  ["agentic AI tooling", "embedded systems", "edge ML"],
    "ask_me_about": ["the last concert I went to (there are many)",
                     "the weirdest thing I've made a microcontroller do"],
    "fun_fact":  "I built Fruit Ninja on a microcontroller, then soldered "
                 "the board it runs on — buying one felt like cheating 🍉",
}
```

I work in the overlap between **embedded systems** and **machine learning** — close
enough to the hardware to care about clock cycles, close enough to the models to
care about what they get wrong. I like problems where the answer has to survive
contact with real hardware.

Being a **first-gen student** taught me to reverse-engineer systems nobody
explained to me, which is conveniently most of engineering. I tend to chase ideas
all the way to something that actually *works* — my offline translation tool
ended up with real users filing feature requests, still the most fun feedback
I've gotten.

<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->

## ✿ what I built at AWS

> *SWE Intern · GenAI Developer Tools · Summer 2026 · TypeScript, Java, MCP, Lambda, CloudWatch*

**🤖 A self-augmenting agent runtime.** Today's LLM agents are stuck with whatever
tools they had at startup. I removed that constraint — a proxy that spawns and
lifecycle-manages child **MCP** servers as live subprocesses, with namespaced
routing, handshake timeouts, crash detection, and automatic cleanup. An agent can
now **install a capability and use it mid-session, with no restart.**

**🔍 Made a ~4,000-server enterprise registry agent-accessible.** Designed, built,
and validated an end-to-end agentic toolchain (**3 services, ~200 automated
tests**) that turns a human-only CLI into a self-service capability layer, so
coding agents can autonomously discover, install, and operate tools.

**⚡ Context-budget-aware retrieval, ~200× faster warm.** A BM25 + fuzzy-matching
index with relevance ranking, TTL caching, and harness-tuned result caps —
serving warm queries in **under 10ms** versus a **~2s** cold build, so the agent
picks relevant tools *without* flooding its context window.

**🔒 Hardened it against prompt injection and tool poisoning.** Untrusted-output
handling, input allowlisting, shell-free execution, a non-repudiation audit log,
and least-privilege scoping that limits each bundled dependency to an allowlisted
subset of tools — all designed under a **generative-AI threat model**.

**📈 Serverless telemetry that can't break the thing it measures.** A Lambda +
CloudWatch pipeline with a lazy, coalescing in-process buffer and a fail-safe
flush, so observability can never add latency to — or fail — a tool call.

<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->

## ✿ things I've built

> The full write-ups, with the engineering detail, live on **[kaitlynchen.dev →](https://kaitlynchen.dev)**

<br/>

### 🥇 Ctrl+Meet — *we won the whole hackathon*

**Grand prize · Amazon's internal hackathon · 190+ engineers**
&nbsp;·&nbsp; [**`view repo →`**](https://github.com/kcitlyn/ctrl-meet)

Not a track, not a side category — **the whole thing.** A cohort-wide peer vote
narrowed the field, then a panel of **Amazon L8 senior leaders** named ours the
**single best build of the entire hackathon.**

A cross-team intern matchmaking platform, shipped on **real AWS behind SSO** — not
a localhost demo.

**The matching engine**
- Scores candidates by **Gower similarity**
- **Auto-weights each question by its entropy**, so questions everyone answers identically carry no signal
- **Gumbel-top-k** sampling + **MMR re-ranking** → a genuinely varied slate, not five clones of you
- A **93-chunk RAG** onboarding bot on Titan embeddings, guaranteed to cite a real doc

**What I owned**
- The **two-sided invite protocol** — strict sender/recipient role separation + cross-device sync, so neither side can accept its own invite
- Read receipts that only fire on a real human open
- Calendar booking, searchable org/city/building pickers, match filtering
- **SigV4 hand-rolled in pure Node crypto** (post-win) — the build sandbox blocked network access, so the AWS SDK client wasn't available

> 🥇 **50 of 109 commits · 138 of 157 tests** — the most of anyone on the team, on either count.

`React` `Lambda` `DynamoDB` `Bedrock` `Titan` `API Gateway` `CDK` `SigV4` `RAG` `Vitest`

<br/>

### 🚗 Texas EcoCar — *ML steering controller for an autonomous vehicle*

Replaced a gain-scheduled PID with a **Gaussian Process** controller — no more
manual calibration, same tracking performance.

- **0.23 m RMSE** lane tracking
- Plant model trained on 1,500 samples in **26 s** → **0.0004 rad** accuracy
- Used the GP's *own* prediction variance as a live confidence metric: an **11,600× variance spike** flags out-of-envelope operation and triggers automatic fallback to proportional control
- **678,000-point** system-ID pipeline (6 speeds × 4 maneuvers); uncertainty bounds validated at **100% coverage within 2σ**

`C/C++` `MATLAB/Simulink` `Python` `Controls`

<br/>

### 🎙️ PolyScribe — *offline transcription + translation, with real users* ⭐13

[**`view repo →`**](https://github.com/kcitlyn/PolyScribe_Desktop)

Speech-to-text and translation across **20+ languages**, running entirely
locally — no cloud, no API keys, no data leaving your machine. A real-time
**multithreaded producer/consumer** pipeline (audio → Vosk STT → Argos NMT → TTS)
with structured exports and fault recovery for device/model failures.

**Open-sourced, and external users started filing feature requests.**

`Python` `Vosk` `Argos` `pyttsx3`

<br/>

### 🩺 edgedoctor — *why did my model break on the edge?*  *(in progress)*

[**`view repo →`**](https://github.com/kcitlyn/edgedoctor)

Profiles a model against target hardware and surfaces the *real* bottleneck —
quantization mismatches, unsupported ops, memory pressure — instead of leaving
you to guess.

`Python` `Edge AI` `ML Tooling`

<br/>

### 🚄 Texas Guadaloop — *hyperloop pod firmware*

Multi-channel **STM32** sensor acquisition using **ADC + DMA circular buffering**
for real-time Hall-effect speed measurement, with a voltage-to-Gauss calibration
pipeline derived from datasheet characterization. Documented the pod-wide
embedded architecture — **9 distributed STM32 nodes**, CAN bus routing topology,
and a LoRa telemetry link to the ground station — as the team-wide interface
reference.

`C` `STM32` `CAN` `ADC/DMA` `UART`

<br/>

### and a few more

| | |
|---|---|
| 👤 **[TrainYourFace](https://github.com/kcitlyn/TrainYourFace)** | Real-time multi-face ID from **128-dim ResNet** embeddings, fully offline, with a tunable false-accept vs. missed-ID threshold. `Python` `OpenCV` `dlib` |
| 🌌 **Astrarium** · *HackTX 2025* | FastAPI + PostgreSQL LLM backend with structured-output validation and timeout/fallback guards, so flaky model latency never takes the app down. `FastAPI` `PostgreSQL` `Next.js` |
| 🍉 **Fruit Ninja on a microcontroller** | On a PCB I designed, printed, and soldered myself — because I wanted to know if I could. `ARM Cortex-M0` `C` `KiCad` |

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

## ✿ how I work

<table>
<tr>
<td width="33%" valign="top" align="center">

**🔬 I trust measurements over vibes**

The GP fault detector exists because I checked *when* the model was wrong, not
just how often. Same instinct behind validating uncertainty bounds at 100%
coverage within 2σ.

</td>
<td width="33%" valign="top" align="center">

**🧱 I build things that fail safely**

Fallback to proportional control. Fail-safe telemetry flush. Structured-output
guards. Crash detection and cleanup. If it can break, I'd rather it break
predictably.

</td>
<td width="33%" valign="top" align="center">

**🚢 I finish things**

Deployed on real AWS, not localhost. Open-sourced and maintained for actual
users. 138 of 157 tests. Shipping is the part where you find out.

</td>
</tr>
</table>

<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->

## ✿ recognition

| | |
|---|---|
| 🏆 | **1st Place — Amazon Internal Hackathon** · winning team among **190+ engineers**, cleared a cohort-wide peer vote and chosen by a panel of Amazon L8 senior leaders |
| 🌸 | **NCWIT Aspirations in Computing** · National Honorable Mention **&** Houston Affiliate Winner |
| 🎓 | **Engineering Honors** · UT Austin Cockrell School — Computer Architecture & Embedded Systems |
| 💛 | **Engineering Honors Scholarship** |
| ✨ | **National First-Gen Recognition** |

<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->

## ✿ currently

- 🔭 **building** — [`edgedoctor`](https://github.com/kcitlyn/edgedoctor), so you can tell *why* your model got slower on the edge instead of guessing
- 🌱 **learning** — how far I can push real models onto small hardware before they stop being useful
- 💌 **looking for** — SWE / ML / embedded / edge-AI internships
- 🎧 **outside of code** — more concerts than is reasonable, sudoku patterns, hiking, and a steady rotation of Raspberry Pi projects

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
