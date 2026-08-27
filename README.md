## Yiğitcan

I write code that sits between machine learning and systems work. Lately that
has meant local vision models driving hardware, GPU kernels, and cryptography.

### Some of what I have built

**[yaykut-cryptology](https://github.com/yigaykut/yaykut-cryptology)**

A cipher where the ciphertext carries a mathematical formula's identity and its
parameters instead of plain text. There are three layers. The engine is
deterministic and does the encryption. A small neural network sits beside it as
an auditor, trying to tell one ciphertext from another, and it never touches
the cipher path. The third layer answers questions about the formula corpus.

The repository also holds a constant-time X25519 core written in C, a fuzzer
that follows branch coverage through `sys.monitoring`, a cycle-level timing
harness, and a tool that reads the compiler's assembly output to check the
constant-time code survived optimisation. There are 29 decision records
explaining the reasoning, and the audit document says plainly which claims were
measured and which were not.

**[GPU-Accelerated-Template-Matching](https://github.com/yigaykut/GPU-Accelerated-Template-Matching)**

Normalised cross-correlation template matching, written as PyTorch GPU kernels.

**[Vision-Guided-4-Axis-Robot-Arm-with-Object-Detection](https://github.com/yigaykut/Vision-Guided-4-Axis-Robot-Arm-with-Object-Detection)**

A four-axis arm that finds an object, tracks it and picks it up. A local Qwen
vision model does the seeing, an Arduino Uno drives the servos.

**[Animatronic-Eye-Mechanism](https://github.com/yigaykut/Animatronic-Eye-Mechanism)**

An eye that follows what the camera sees, again with a local Qwen model and an
Arduino behind it.

**[stock-ranking-engine](https://github.com/yigaykut/stock-ranking-engine)**

A screener that ranks US small and mid cap equities against 28 factors, run
daily.

### What I am interested in

Writing code whose timing does not depend on secrets, and then measuring
whether that is actually true rather than assuming it. Fuzzing. Keeping
statistical models away from the parts of a system that have to be exactly
right.
