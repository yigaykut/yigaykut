<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0b1a2e,100:1f6feb&height=160&section=header&text=Yi%C4%9Fitcan&fontColor=ffffff&fontSize=46&fontAlignY=34&desc=machine%20learning%20next%20to%20systems%20work&descAlignY=56&descSize=14" alt="" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="" />
  <img src="https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black" alt="" />
  <img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white" alt="" />
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" alt="" />
  <img src="https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white" alt="" />
  <img src="https://img.shields.io/badge/Arduino-00979D?style=flat-square&logo=arduino&logoColor=white" alt="" />
  <img src="https://komarev.com/ghpvc/?username=yigaykut&style=flat-square&color=1f6feb&label=views" alt="" />
</p>

I write code that sits between machine learning and systems work. Lately that has meant local vision models driving hardware, GPU kernels, and cryptography.

### Some of what I have built

**[yaykut-cryptology](https://github.com/yigaykut/yaykut-cryptology)** &nbsp;`Python` `C`

A cipher where the ciphertext carries a mathematical formula's identity and its parameters instead of plain text. Three layers: a deterministic engine that does the encryption, a small neural network beside it as an auditor that never touches the cipher path, and a third layer that answers questions about the formula corpus.

It also holds a constant-time X25519 core in C, a fuzzer that follows branch coverage through `sys.monitoring`, a cycle-level timing harness, and a tool that reads the compiler's assembly output to check the constant-time code survived optimisation. There are 29 decision records, and the audit document says plainly which claims were measured and which were not.

**[GPU-Accelerated-Template-Matching](https://github.com/yigaykut/GPU-Accelerated-Template-Matching)** &nbsp;`PyTorch`

Normalised cross-correlation template matching, written as PyTorch GPU kernels.

**[Vision-Guided-4-Axis-Robot-Arm](https://github.com/yigaykut/Vision-Guided-4-Axis-Robot-Arm-with-Object-Detection)** &nbsp;`Python` `C++`

A four-axis arm that finds an object, tracks it and picks it up. A local Qwen vision model does the seeing, an Arduino Uno drives the servos.

**[Animatronic-Eye-Mechanism](https://github.com/yigaykut/Animatronic-Eye-Mechanism)** &nbsp;`Python` `C++`

An eye that follows what the camera sees, again with a local Qwen model and an Arduino behind it.

**[stock-ranking-engine](https://github.com/yigaykut/stock-ranking-engine)** &nbsp;`Python`

A screener that ranks US small and mid cap equities against 28 factors, run daily.

<p align="center">
  <img height="150" src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=yigaykut&theme=github_dark" alt="" />
  <img height="150" src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=yigaykut&theme=github_dark" alt="" />
</p>

### What I am interested in

Writing code whose timing does not depend on secrets, and then measuring whether that is actually true rather than assuming it. Fuzzing. Keeping statistical models away from the parts of a system that have to be exactly right.
