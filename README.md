# Learning Phonetic Context-Dependent Viseme for Enhancing Speech-Driven 3D Facial Animation
### [Project Page](https://kimhyungkyu-1208.github.io/interspeech25/) | [Paper](#) | [Video](#) [![arXiv](https://img.shields.io/badge/arXiv-24XX.XXXXX-b31b1b.svg)](https://arxiv.org/abs/your-paper-id) [![GitHub](https://img.shields.io/github/stars/kimhyungkyu-1208/interspeech25?style=social)](https://github.com/kimhyungkyu-1208/interspeech25)

**Interspeech 2025 (Accepted)**

[Hyung Kyu Kim](https://kimhyungkyu-1208.github.io/HYUNG-KYU-KIM/) , [Hak Gu Kim]([#](https://hgkimcau.github.io/)) <br>

This work addresses the subtle yet critical issues of jitter and unnatural lip movements in existing speech-driven 3D facial animations. We introduce a novel loss function, the Phonetic Context-aware Loss, which explicitly models the influence of preceding and following phonemes (coarticulation) to generate smoother and more realistic results.

## What is Phonetic Context-aware Loss?

Traditional speech-driven 3D facial animation models are trained by minimizing the geometric error (e.g., MSE Loss) between the generated mesh and the ground truth on a frame-by-frame basis. This approach often fails to capture the continuous nature of facial motion, overlooking the phenomenon of 'coarticulation'—where the articulation of a sound is affected by its neighbors. This results in jittery and perceptually unnatural animations.

Our **Phonetic Context-aware Loss (<span class="math-inline">\\mathcal\{L\}\_\{pc\}</span>)** is a novel objective function that addresses this limitation. It computes a "viseme coarticulation weight" that quantifies how much a viseme's articulation is influenced by its phonetic context. By applying this weight, the model learns to pay more attention to frames with significant articulatory transitions, resulting in smoother, more natural, and intelligible 3D facial animations.

## Citation

If you find our work useful, please consider citing our paper:
```bibtex
@inproceedings{kim2025learning,
  title={Learning Phonetic Context-Dependent Viseme for Enhancing Speech-Driven 3D Facial Animation},
  author={Hyung Kyu Kim and Hak Gu Kim},
  booktitle={Proc. INTERSPEECH},
  year={2025},
  organization={ISCA}
}
```

## Acknowledgments
Parts of this project page were adopted from the [Nerfies](https://nerfies.github.io/) page.

## Website License
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
