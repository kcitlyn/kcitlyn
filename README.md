<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:ffd6e8,50:ffb3d1,100:f9a8d4&height=180&section=header&text=hi,%20I'm%20Kaitlyn%20✿&fontSize=44&fontColor=4a2540&fontAlignY=34&desc=ECE%20@%20UT%20Austin%20·%20I%20make%20software%20touch%20the%20real%20world&descSize=16&descAlignY=56&descAlign=50" width="100%" />

<a href="https://kaitlynchen.dev">
  <img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=500&size=21&duration=3400&pause=900&color=F9A8D4&center=true&vCenter=true&width=620&lines=SWE+Intern+%40+AWS+%C2%B7+GenAI+Developer+Tools;STM32+firmware+%E2%86%92+agentic+AI+tooling;1st+place+%F0%9F%8F%86+Amazon+hackathon+%C2%B7+190%2B+engineers;close+to+the+metal%2C+curious+about+the+models" alt="what I do" />
</a>

<br/>

[![Portfolio](https://img.shields.io/badge/✿_kaitlynchen.dev-FFB3D1?style=for-the-badge&logoColor=4A2540&labelColor=FFD6E8)](https://kaitlynchen.dev)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-F9A8D4?style=for-the-badge&logo=linkedin&logoColor=4A2540&labelColor=FFD6E8)](https://www.linkedin.com/in/kaitlynychen)
[![Email](https://img.shields.io/badge/say_hi-FFC1DD?style=for-the-badge&logo=gmail&logoColor=4A2540&labelColor=FFD6E8)](mailto:kcitlynychen@gmail.com)
![Profile views](https://komarev.com/ghpvc/?username=kcitlyn&style=for-the-badge&color=ffb3d1&label=visitors)

</div>

<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->

## ✿ about me

```python
kaitlyn = {
    "role":      "SWE Intern @ AWS — GenAI Developer Tools",
    "school":    "BS Electrical & Computer Engineering, UT Austin",
    "lives_in":  "Austin, TX  ✈  Seattle, WA",
    "works_on":  ["agentic AI tooling", "embedded systems", "edge ML"],
    "ask_me_about": "why your model got slower after you quantized it",
    "fun_fact":  "I built Fruit Ninja on a microcontroller — on a PCB I "
                 "designed, printed, and soldered myself 🍉",
}
```

I work in the overlap between **embedded systems** and **machine learning** — close
enough to the hardware to care about clock cycles, close enough to the models to
care about what they get wrong.

Being a **first-gen student** taught me to reverse-engineer systems nobody
explained to me, which is conveniently most of engineering. I tend to chase ideas
all the way to something that actually *works* — my offline translation tool
ended up with real users requesting features, still the most fun feedback I've
gotten.

<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->

## ✿ what I've been building

<table>
<tr>
<td width="50%" valign="top">

### 🏆 Ctrl+Meet
**1st place — Amazon internal hackathon**

Beat out **190+ competing engineers**: cleared a cohort-wide peer vote, then a
panel of **Amazon L8 senior leaders** picked our build as the best in the field.

An intern-matchmaking platform, shipped on real AWS instead of localhost.
The recommender scores candidates by **Gower similarity** with **entropy
auto-weighting**, then **Gumbel-top-k** sampling + **MMR re-ranking** so your
matches are genuinely varied. Plus a RAG onboarding bot on Titan embeddings.

*I wrote 50 of 109 commits and 138 of 157 tests — most of anyone on either.*

`React` `Lambda` `DynamoDB` `Bedrock` `RAG` `CDK`

</td>
<td width="50%" valign="top">

### 🎙️ [PolyScribe](https://github.com/kcitlyn/PolyScribe_Desktop) ⭐13
**Fully-offline transcription + translation**

Speech-to-text and text-to-speech across **20+ languages**, running entirely
locally — no cloud, no API keys, no data leaving your machine.

Open-sourced and picked up by real external users who started filing feature
requests. My most-starred repo.

`Python` `Vosk` `Argos`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🚗 Texas EcoCar
**ML steering controller for an autonomous vehicle**

Replaced a gain-scheduled PID with a **Gaussian Process** controller — killed the
manual calibration while holding **0.23 m RMSE** lane tracking.

Then used the GP's own prediction variance as a live fault detector: an
**11,600× variance spike** flags out-of-envelope operation and triggers fallback
to proportional control. Trained on a 678k-point pipeline.

`C/C++` `MATLAB/Simulink` `Python`

</td>
<td width="50%" valign="top">

### 🩺 [edgedoctor](https://github.com/kcitlyn/edgedoctor)
**Why did my model break on the edge?** *(in progress)*

Profiles a model against target hardware and surfaces the *real* bottleneck —
quantization mismatches, unsupported ops, memory pressure — instead of leaving
you to guess.

`Python` `Edge AI` `ML Tooling`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🚄 Texas Guadaloop
**Hyperloop pod firmware**

Multi-channel **STM32** sensor acquisition using **ADC + DMA circular
buffering** for real-time Hall-effect speed measurement, with a
voltage-to-Gauss calibration pipeline built from datasheet characterization.

Documented the pod-wide architecture — 9 distributed STM32 nodes, CAN routing
topology, LoRa telemetry — as the team-wide interface reference.

`C` `STM32` `CAN` `DMA` `UART`

</td>
<td width="50%" valign="top">

### 👤 [TrainYourFace](https://github.com/kcitlyn/TrainYourFace)
**Offline face recognition**

Real-time multi-face identification with **128-dimensional ResNet
embeddings** — fully offline, with in-terminal capture and training.

`Python` `OpenCV` `dlib`

</td>
</tr>
</table>

<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->

## ✿ my toolbox

<div align="center">

**languages**

<img src="https://skillicons.dev/icons?i=py,c,cpp,ts,js,matlab,bash,latex&theme=light" />

**AI / agentic**

`MCP` · `LLM agents` · `RAG` · `evals & benchmarking` · `structured-output validation` · `prompt-injection defense`

**embedded & hardware**

<img src="https://skillicons.dev/icons?i=arduino,raspberrypi&theme=light" />

`STM32` · `ARM Cortex-M0` · `CAN` · `I2C/SPI/UART` · `ADC/DMA` · `real-time systems` · `PCB layout` · `KiCad` · `LTSpice` · `oscilloscope`

**ML / perception**

`OpenCV` · `Gaussian Process regression` · `dlib` · `ResNet` · `system identification` · `real-time video inference`

**web, cloud & systems**

<img src="https://skillicons.dev/icons?i=react,nextjs,tailwind,fastapi,postgres,aws,docker,linux,git,cmake&theme=light" />

</div>

<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->

## ✿ recognition

| | |
|---|---|
| 🏆 | **1st Place — Amazon Internal Hackathon** · winning team among 190+ engineers, chosen by a panel of Amazon L8 senior leaders |
| 🌸 | **NCWIT Aspirations in Computing** · National Honorable Mention & Houston Affiliate Winner |
| 🎓 | **Engineering Honors Scholarship** · UT Austin |
| ✨ | **National First-Gen Recognition** |

<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->

## ✿ the stats

<div align="center">

<img src="https://github-readme-streak-stats.herokuapp.com/?user=kcitlyn&theme=material-palenight&hide_border=true&background=0D1117&stroke=F9A8D4&ring=FFB3D1&fire=FFD6E8&currStreakLabel=F9A8D4&sideLabels=FFC1DD&dates=9A9AA5" width="70%" alt="streak" />

<img src="https://github-readme-activity-graph.vercel.app/graph?username=kcitlyn&bg_color=0D1117&color=FFD6E8&line=F9A8D4&point=FFFFFF&area=true&area_color=FFB3D1&hide_border=true&custom_title=my%20commit%20rhythm" width="95%" alt="activity graph" />

</div>

<!-- ✿ ─────────────────────────────────────────────────────────────── ✿ -->

## ✿ currently

- 🔭 **building** — agentic AI developer tooling at AWS, and `edgedoctor` on the side
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
