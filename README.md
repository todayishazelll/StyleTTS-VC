# StyleTTS-VC: One-Shot Voice Conversion by Knowledge Transfer from Style-Based TTS Models

### Yinghao Aaron Li, Cong Han, Nima Mesgarani
Paper: [https://arxiv.org/abs/2212.14227](https://arxiv.org/abs/2212.14227)

Audio samples: [https://styletts-vc.github.io/](https://styletts-vc.github.io/)


# Model Summary
(models_stats.py)

| Component         | Total Parameters | Trainable Parameters | Non-trainable Parameters | Total Mult-adds (M/G) | Input Size (MB) | Forward/Backward Pass Size (MB) | Params Size (MB) | Estimated Total Size (MB) | Running Time (s) |
|-------------------|------------------|-----------------------|--------------------------|-----------------------|-----------------|----------------------------------|-------------------|---------------------------|--------------------|
| **Mel Encoder**    | 4,529,408           | 4,529,408                | 0                        | 2.08 G                | 0.06            | 10.22                             | 18.12              | 28.40                      | 0.0969 |
| **Linear Proj**    | 91,314           | 91,314                | 0                        | 8.77 M                | 0.20            | 0.14                             | 0.37              | 0.70                      | 0.0149 |
| **Text Encoder**   | 5,606,400        | 5,606,400             | 0                        | 82.75 G               | 0.00            | 3.28                             | 22.43             | 25.70                     | 0.0840 |
| **Style Encoder**  | 13,845,440       | 13,845,440            | 0                        | 6.72 G                | 0.06            | 60.98                            | 55.38             | 116.43                    | 0.1507 |
| **Discriminator**  | 13,835,180       | 13,835,180            | 0                        | 6.72 G                | 0.06            | 60.98                            | 55.34             | 116.38                    | 0.1170 |
| **Decoder**        | 32,719,026       | 32,719,026            | 0                        | 55.54 G               | 0.20            | 0.22                             | 0.30              | 0.72                      | 0.1560 |
| **Pitch Extractor**        | 5,248,067       | 5,248,067            | 0                        | 7.24 G               | 0.06            | 119.93                             | 8.38              | 128.37                      | 0.1984 |
| **Text Aligner**        | 7,865,252       | 7,865,252            | 0                        | 5.83 G               | 0.06            | 13.06                             | 31.46              | 44.58                      | 0.3031 |

### Total Model Summary:
- **Total Parameters**: 83,740,087
- **Total Mult-adds**: 166.89 G
- **Total Running Time**: 1.121 s

Mel Encoder, Linear Proj, Text Encoder, Style Encoder, Decoder, Pitch Extractor, Text Aligner: Used for both training and inference.

Discriminator: Used primarily for training.
