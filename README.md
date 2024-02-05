# Personalization as a Shortcut for Few-Shot Backdoor Attack against Text-to-Image Diffusion Models
This is the official repository of [Personalization as a Shortcut for Few-Shot Backdoor Attack against Text-to-Image Diffusion Models](https://arxiv.org/pdf/2305.10701.pdf).
The paper is accepted by AAAI 2024.

[![arXiv](https://img.shields.io/badge/arXiv-2305.10701-b31b1b.svg)]([https://arxiv.org/abs/2305.10701](https://arxiv.org/pdf/2305.10701.pdf))

> **Personalization as a Shortcut for Few-Shot Backdoor Attack against Text-to-Image Diffusion Models**<br>
> Yihao Huang, Felix Juefei-Xu, Qing Guo, Jie Zhang, Yutong Wu, Ming Hu, Tianlin Li, Geguang Pu, Yang Liu <br>

>**Abstract**: <br>
> Although recent personalization methods have democratized high-resolution image synthesis by enabling swift concept acquisition with minimal examples and lightweight computation, they also present an exploitable avenue for high accessible backdoor attacks. This paper investigates a critical and unexplored aspect of text-to-image (T2I) diffusion models - their potential vulnerability to backdoor attacks via personalization. Our study focuses on a zero-day backdoor vulnerability prevalent in two families of personalization methods, epitomized by Textual Inversion and DreamBooth.Compared to traditional backdoor attacks, our proposed method can facilitate more precise, efficient, and easily accessible attacks with a lower barrier to entry. We provide a comprehensive review of personalization in T2I diffusion models, highlighting the operation and exploitation potential of this backdoor vulnerability. To be specific, by studying the prompt processing of Textual Inversion and DreamBooth, we have devised dedicated backdoor attacks according to the different ways of dealing with unseen tokens and analyzed the influence of triggers and concept images on the attack effect. Through comprehensive empirical study, we endorse the utilization of the nouveau-token backdoor attack due to its impressive effectiveness, stealthiness, and integrity, markedly outperforming the legacy-token backdoor attack.


# Details
The method is based on [Textual Inversion](https://textual-inversion.github.io/) and [Dreambooth](https://dreambooth.github.io/).
We follow the code implemented on hugging face 
- https://github.com/huggingface/notebooks/blob/main/diffusers/sd_textual_inversion_training.ipynb
- https://github.com/huggingface/notebooks/blob/main/diffusers/sd_dreambooth_training.ipynb

It is very easy to construct the backdoor, you only need to provide mismatched text-image pairs to the code above.

# References
```
@article{huang2023zero,
  title={Personalization as a Shortcut for Few-Shot Backdoor Attack against Text-to-Image Diffusion Models},
  author={Yihao Huang, Felix Juefei-Xu, Qing Guo, Jie Zhang, Yutong Wu, Ming Hu, Tianlin Li, Geguang Pu, Yang Liu},
  journal={arXiv preprint arXiv:2305.10701},
  year={2023}
}
```
