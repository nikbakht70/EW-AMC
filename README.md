# EW-AMC
Fundamental Innovations of the Project
1. Moving from a Single-Frame to a Multi-Frame Perspective
Most previous systems analyzed each piece of signal separately, like someone watching a movie frame by frame, without considering the connections between the frames. But real signals have a continuous story. The changes from one frame to the next provide important clues. The current code solves this problem by using five consecutive frames (five consecutive images of the signal film). This allows the model to understand not only the content of each frame, but also how that content changes over time. Is the signal changing slowly (as in phase modulation) or abruptly (as in amplitude modulation)? These temporal patterns are key to recognizing many modulations.
2. Attention Mechanism: Focusing on the Most Important Parts
One of the interesting innovations in this project is the use of a temporal attention mechanism. This idea is inspired by the way the human brain works. When we look at a scene, we don’t pay equal attention to everything. We focus on the most important parts. In this code, the model also learns which frames provide it with more information. In some situations, the middle frames may have the most information, or perhaps the early frames. The model dynamically gives more weight to the more important frames and less attention to the less important frames. This not only increases accuracy, but also makes the model more efficient - it focuses computational resources on the key parts.
3. Programmatic Training: Learning Step by Step Like a Human
Perhaps the most beautiful part of this project is its training strategy. The code uses a concept called “programmatic training,” which is inspired by the way humans learn. We teach children simple things first (reading simple words), then more complex concepts (sentence building), and finally advanced things (writing).
This code does exactly that:
• Stage 1: First, it trains with clear and strong signals (with a high signal-to-noise ratio).
• Stage 2: Then it practices with moderate signals.
• Stage 3: And finally, it works with weak and noisy signals.
This approach has several important advantages:

Faster learning, the model learns the basics first in easy conditions.
Better performance in difficult conditions, as the model gradually encounters more difficult conditions, it can cope better with them.
Error reduction, this method helps the model not fall into the trap of common misdiagnoses.

Context information integration: using all available clues
Another important innovation of this code is the intelligent use of context information. In traditional systems, only the signal itself was analyzed. But this code also brings a very valuable additional piece of information into the equation: the signal-to-noise ratio (SNR). It's like knowing what the background noise level is when you're listening to that conversation at a loud party. This additional information helps the model better interpret the signal. If it knows there's a lot of noise, it adjusts its expectations of the signal's clarity, making it less likely that small changes will be part of the useful information.
