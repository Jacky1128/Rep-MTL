<div align="center">

# Rep-MTL: Unleashing the Power of Representation-level Task Saliency for Multi-Task Learning

<!-- ICCV 2025 Highlight -->
<div align="center" style="margin: 35px 0;">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=16&height=150&section=header&text=ICCV%202025%20Highlight%20Paper&fontSize=30&fontColor=fff&animation=fadeIn&fontAlignY=38&desc=Honolulu%2C%20Hawaii&descSize=19&descAlignY=62&fontFamily=Playfair+Display" width="100%"/>
</div>

<p align="center">
  <a href="https://arxiv.org/abs/2507.21049" style="text-decoration: none;" target="_blank">
    <img src="https://img.shields.io/badge/arXiv-2507.21049-b31b1b.svg?style=for-the-badge&logo=arxiv&logoColor=white" alt="arXiv"/>
  </a>
  <a href="https://jacky1128.github.io/RepMTL/" style="text-decoration: none;" target="_blank">
    <img src="https://img.shields.io/badge/PROJECT-RepMTL-blue.svg?style=for-the-badge&logo=firefox&logoColor=white" alt="Project Page"/>
  </a>
  <a href="https://huggingface.co/papers/2507.21049" style="text-decoration: none;" target="_blank">
    <img src="https://img.shields.io/badge/🤗%20Hugging Face-DailyPapers Top3-yellow.svg?style=for-the-badge&logoColor=white" alt="Demo"/>
  </a>
</p>

<!-- Authors -->
**<a href="https://jacky1128.github.io" target="_blank">Zedong Wang</a><sup>1</sup>, <a href="https://lupin1998.github.io" target="_blank">Siyuan Li</a><sup>2</sup>, <a href="https://www.danxurgb.net" target="_blank">Dan Xu</a><sup>1</sup>**

<sup>1</sup>The Hong Kong University of Science and Technology, <sup>2</sup>Zhejiang University

</div>

<br/>
<br/>

<!-- Teaser -->
<div align="center">
  <img src="img/Teaser.png" alt="Rep-MTL Method Overview" width="80%"/>
  <p><em><strong>(a)</strong> Most existing MTL optimization methods focus on addressing conflicts in parameter updates. <strong>(b)</strong> Rep-MTL instead leverages task saliency in shared representation space to explicitly facilitate cross-task information sharing while preserving task-specific signals via regularization, without modifications to either the underlying optimizers or model architectures.</em></p>
</div>



## Overview

Rep-MTL is a representation-level regularization method for multi-task learning that introduces task saliency-based objectives to encourage inter-task complementarity via Cross-task Saliency Alignment (CSA) while mitigating negative transfer among tasks via Task-specific Saliency Regulation (TSR).



## Benchmarks

We evaluate Rep-MTL on several challenging MTL benchmarks spanning diverse computer vision scenarios:

| Dataset | Tasks | Scenario | Download |
|---------|-------|--------|----------|
| <a href="https://cs.nyu.edu/~silberman/datasets/nyu_depth_v2.html" target="_blank">NYUv2</a> | SemSeg + Depth Est. + Surface Normal Pred. | Indoor Dense Prediction | <a href="https://cs.nyu.edu/~silberman/datasets/nyu_depth_v2.html" target="_blank">Link</a> |
| <a href="https://www.cityscapes-dataset.com/" target="_blank">CityScapes</a> | SemSeg + Depth Est. | Outdoor Dense Prediction | <a href="https://www.cityscapes-dataset.com/downloads/" target="_blank">Link</a> |
| <a href="https://people.eecs.berkeley.edu/~jhoffman/domainadapt/" target="_blank">Office-31</a> | Image Classification (31 classes) | Domain Adaptation | <a href="https://people.eecs.berkeley.edu/~jhoffman/domainadapt/" target="_blank">Link</a> |
| <a href="https://www.hemanthdv.org/officeHomeDataset.html" target="_blank">Office-Home</a> | Image Classification (65 classes) | Domain Adaptation | <a href="https://www.hemanthdv.org/officeHomeDataset.html" target="_blank">Link</a> |



## Updates
- **[July 24, 2025]** 🎉 Rep-MTL was selected as **ICCV 2025 Highlight**! We are working on cleaning and organizing our codebase. Stay tuned!
- **[June 26, 2025]** Rep-MTL was accepted to **ICCV 2025**, with final ratings: 5/5/6 (out of 6).


## Contact

For questions or research discussions, please contact <a href="https://jacky1128.github.io" target="_blank">Zedong Wang</a> at `zedong.wang@connect.ust.hk`.



## BibTeX


```bibtex
@inproceedings{iccv2025repmtl,
  title={Rep-MTL: Unleashing the Power of Representation-level Task Saliency for Multi-Task Learning},
  author={Wang, Zedong and Li, Siyuan and Xu, Dan},
  booktitle={IEEE/CVF International Conference on Computer Vision (ICCV)},
  year={2025}
}
```


## Acknowledgements

We thank the following great repositories that facilitated our research: <a href="https://github.com/median-research-group/LibMTL" target="_blank">LibMTL</a>, <a href="https://github.com/Cranial-XIX/CAGrad" target="_blank">CAGrad</a>, <a href="https://github.com/lorenmt/mtan" target="_blank">MTAN</a>, <a href="https://github.com/Cranial-XIX/FAMO" target="_blank">FAMO</a>, and <a href="https://github.com/AvivNavon/nash-mtl" target="_blank">Nash-MTL</a>. We also extend our appreciation to many other studies in the community for their foundational contributions that inspired this work.
