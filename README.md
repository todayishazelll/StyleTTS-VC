# StyleTTS-VC: One-Shot Voice Conversion by Knowledge Transfer from Style-Based TTS Models

### Yinghao Aaron Li, Cong Han, Nima Mesgarani
Paper: [https://arxiv.org/abs/2212.14227](https://arxiv.org/abs/2212.14227)

Audio samples: [https://styletts-vc.github.io/](https://styletts-vc.github.io/)


# Model Summary

| Component         | Total Parameters | Trainable Parameters | Non-trainable Parameters | Total Mult-adds (M/G) | Input Size (MB) | Forward/Backward Pass Size (MB) | Params Size (MB) | Estimated Total Size (MB) |
|-------------------|------------------|-----------------------|--------------------------|-----------------------|-----------------|----------------------------------|-------------------|---------------------------|
| **Mel Encoder**    | 91,314           | 91,314                | 0                        | 8.77 M                | 0.20            | 0.14                             | 0.37              | 0.70                      |
| **Text Encoder**   | 5,606,400        | 5,606,400             | 0                        | 82.75 G               | 0.00            | 3.28                             | 22.43             | 25.70                     |
| **Style Encoder**  | 13,845,440       | 13,845,440            | 0                        | 6.72 G                | 0.06            | 60.98                            | 55.38             | 116.43                    |
| **Discriminator**  | 13,835,180       | 13,835,180            | 0                        | 6.72 G                | 0.06            | 60.98                            | 55.34             | 116.38                    |
| **Decoder**        | 32,719,026       | 32,719,026            | 0                        | 55.54 G               | 0.20            | 0.22                             | 0.30              | 0.72                      |

### Total Model Summary:
- **Total Parameters**: 66,097,360
- **Total Mult-adds**: 160.50 G
- **Total Estimated Size**: **259.93 MB**


