# Awesome Human Motion Generation
A curated list of papers and open-source resources focused on Human Motion Generation, intended to keep pace with the anticipated growth and accelerate research in this field.
If you have any additions or suggestions, feel free to contribute. Additional resources like blog posts, videos, etc. are also welcome.

## Table of Contents
- [Datasets](#datasets)
- [Text-to-Motion](#test-to-motion)

<details span>
<summary><b>Update Log:</b></summary>
<br>

**Oct 9, 2024**
- Initial commit
</details>
<br>

## Datasets

### [Big Data, 2016] The KIT Motion-Language Dataset
**Authors**: Matthias Plappert, Christian Mandery, Tamim Asfour
<details span>
<summary><b>Abstract</b></summary>
Linking human motion and natural language is of great interest for the generation of semantic representations of human activities as well as for the generation of robot activities based on natural language input. However, while there have been years of research in this area, no standardized and openly available dataset exists to support the development and evaluation of such systems. We therefore propose the KIT Motion-Language Dataset, which is large, open, and extensible. We aggregate data from multiple motion capture databases and include them in our dataset using a unified representation that is independent of the capture system or marker set, making it easy to work with the data regardless of its origin. To obtain motion annotations in natural language, we apply a crowd-sourcing approach and a web-based tool that was specifically build for this purpose, the Motion Annotation Tool. We thoroughly document the annotation process itself and discuss gamification methods that we used to keep annotators motivated. We further propose a novel method, perplexity-based selection, which systematically selects motions for further annotation that are either under-represented in our dataset or that have erroneous annotations. We show that our method mitigates the two aforementioned problems and ensures a systematic annotation process. We provide an in-depth analysis of the structure and contents of our resulting dataset, which, as of October 10, 2016, contains 3911 motions with a total duration of 11.23 hours and 6278 annotations in natural language that contain 52,903 words. We believe this makes our dataset an excellent choice that enables more transparent and comparable research in this important area.
</details>

[📄 Paper](https://arxiv.org/abs/1607.03827) | [💻 Code](https://motion-annotation.humanoids.kit.edu/dataset/)

## Text-to-Motion

### [ECCV, 2022] TEMOS: Generating diverse human motions from textual descriptions
**Authors**: Mathis Petrovich, Michael J. Black, Gül Varol
<details span>
<summary><b>Abstract</b></summary>
We address the problem of generating diverse 3D human motions from textual descriptions. This challenging task requires joint modeling of both modalities: understanding and extracting useful human-centric information from the text, and then generating plausible and realistic sequences of human poses. In contrast to most previous work which focuses on generating a single, deterministic, motion from a textual description, we design a variational approach that can produce multiple diverse human motions. We propose TEMOS, a text-conditioned generative model leveraging variational autoencoder (VAE) training with human motion data, in combination with a text encoder that produces distribution parameters compatible with the VAE latent space. We show the TEMOS framework can produce both skeleton-based animations as in prior work, as well more expressive SMPL body motions. We evaluate our approach on the KIT Motion-Language benchmark and, despite being relatively straightforward, demonstrate significant improvements over the state of the art. Code and models are available on our webpage.
</details>

[📄 Paper](https://arxiv.org/abs/2204.14109) | [💻 Code](https://github.com/Mathux/TEMOS)

### [ICLR, 2023] Human Motion Diffusion Model 
**Authors**: Guy Tevet, Sigal Raab, Brian Gordon, Yonatan Shafir, Daniel Cohen-Or, Amit H. Bermano
<details span>
<summary><b>Abstract</b></summary>
Natural and expressive human motion generation is the holy grail of computer animation. It is a challenging task, due to the diversity of possible motion, human perceptual sensitivity to it, and the difficulty of accurately describing it. Therefore, current generative solutions are either low-quality or limited in expressiveness. Diffusion models, which have already shown remarkable generative capabilities in other domains, are promising candidates for human motion due to their many-to-many nature, but they tend to be resource hungry and hard to control. In this paper, we introduce Motion Diffusion Model (MDM), a carefully adapted classifier-free diffusion-based generative model for the human motion domain. MDM is transformer-based, combining insights from motion generation literature. A notable design-choice is the prediction of the sample, rather than the noise, in each diffusion step. This facilitates the use of established geometric losses on the locations and velocities of the motion, such as the foot contact loss. As we demonstrate, MDM is a generic approach, enabling different modes of conditioning, and different generation tasks. We show that our model is trained with lightweight resources and yet achieves state-of-the-art results on leading benchmarks for text-to-motion and action-to-motion. this https URL .
</details>

[📄 Paper](https://arxiv.org/abs/2209.14916) | [💻 Code](https://github.com/GuyTevet/motion-diffusion-model)



