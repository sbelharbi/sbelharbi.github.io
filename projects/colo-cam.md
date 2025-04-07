---
layout: home2
permalink: /colo-cam/
title: "CoLo-CAM: Class Activation Mapping for Object Co-Localization in Weakly-Labeled Unconstrained Videos (Pattern Recognition 2025)"
tags: [Weakly-supervised Object Localization, Weakly Labeled Unconstrained Videos, Co-localization, Classactivation Mapping (CAMs), Deep Learning, Convolutional Neural Networks, Code, Github]
comments: false
---
by **Soufiane Belharbi<sup>1</sup>,  Shakeeb Murtaza<sup>1</sup>, Marco Pedersoli<sup>1</sup>, Ismail Ben Ayed<sup>1</sup>, Luke McCaffrey<sup>2</sup>, Eric Granger<sup>1</sup>**

<br />

<sup>1</sup>  LIVIA, ILLS, Dept. of Systems Engineering, ETS Montreal, Canada
<br/>
<sup>2</sup>  Goodman Cancer Research Centre, Dept. of Oncology, McGill University, Montreal, Canada

[![arXiv](https://img.shields.io/badge/arXiv-2406.09168-b31b1b.svg?logo=arxiv&logoColor=B31B1B)](https://arxiv.org/pdf/2303.09044)
[![Github](https://img.shields.io/badge/Github-colo--cam-brightgreen.svg?logo=github)](https://github.com/sbelharbi/colo-cam)
[![DOI](https://img.shields.io/badge/DOI-10.1016/j.patcog.2025.111358-lightgreen?logo=doi&logoColor=FAB70C)](https://doi.org/10.1016/j.patcog.2025.111358)
[![Free Access](https://img.shields.io/badge/Temporary%20Journal%20Free%20Access:%20March--14--2025-blue?logo=openaccess)](https://authors.elsevier.com/a/1kUV-77nKs8lu)



<p style="text-align:center;">

<video src="https://user-images.githubusercontent.com/23446793/225508947-de947dbe-3844-46d9-90f0-19c26216eb46.mp4
" width="320" height="240" controls></video>
<video src="https://user-images.githubusercontent.com/23446793/225508954-3f56e762-b0b6-4731-8517-5b8231cf51f9.mp4
" width="320" height="240" controls></video>
<video src="https://user-images.githubusercontent.com/23446793/225508969-cb8b983f-1d35-4b90-8605-77d9b087bcbc.mp4
" width="320" height="240" controls></video>
<video src="https://user-images.githubusercontent.com/23446793/225508965-5109b095-87de-4ec9-88b9-f527c733f999.mp4
" width="320" height="240" controls></video>
<video src="https://user-images.githubusercontent.com/23446793/226443065-a215c0c1-a3ac-4ca9-8aef-9dcd0790bdd4.mp4
" width="320" height="240" controls></video>
<video src="https://user-images.githubusercontent.com/23446793/226443290-8de25beb-33f9-4de6-aa66-46dd2a8f008a.mp4
" width="320" height="240" controls></video>

</p>


<br />

<p align="center">
  <a href="/material/colo-cam/demo.png">
    <img src="{{ site.url }}/material/colo-cam/demo.png" alt="CoLo-CAM: Demo" width="800">
  </a>
</p>


<br />

```latex
@article{belharbi2025colocam,
  title={CoLo-CAM: Class Activation Mapping for Object Co-Localization in Weakly-Labeled Unconstrained Videos},
  author={Belharbi, S. and Murtaza, S. and Pedersoli, M. and Ben Ayed, I. and
  McCaffrey, L. and Granger, E.},
  journal={Pattern Recognition},
  volume={162},
  pages={111358},
  year={2025}
}
```


<!-- <a href="javascript:toggleBibtex('belharbi24-sr-caco-2')">[BibTeX]</a>

<div id="bib_belharbi24-sr-caco-2" class="bibtex noshow">
<pre>
@inproceedings{belharbi24-sr-caco-2,
  title={SR-CACO-2: A Dataset for Confocal Fluorescence Microscopy Image Super-Resolution},
  author={Belharbi, S. and Whitford, M.K.M. and Hoang, P. and Murtaza, S.
  and McCaffrey, L. and Granger, E.},
  booktitle={NeurIPS},
  year={2024}
}
</pre>
</div> -->



### Abstract

Leveraging spatiotemporal information in videos is critical for weakly supervised video object localization (WSVOL) tasks. However, state-of-the-art methods only rely on visual and motion cues, while discarding discriminative information, making them susceptible to inaccurate localizations. Recently, discriminative models have been explored for WSVOL tasks using a temporal class activation mapping (CAM) method. Although their results are promising, objects are assumed to have limited movement from frame to frame, leading to degradation in performance for relatively long-term dependencies.
This paper proposes a novel CAM method for WSVOL that exploits spatiotemporal information in activation maps during training without constraining an object's position. Its training relies on <i>Co</i>-<i>Lo</i>calization, hence, the name *CoLo-CAM*.
Given a sequence of frames, localization is jointly learned based on color cues extracted across the corresponding maps, by assuming that an object has similar color in consecutive frames. CAM activations are constrained to respond similarly over pixels with similar colors, achieving co-localization. This improves localization performance because the joint learning creates direct communication among pixels across all image locations and over all frames, allowing for transfer, aggregation, and correction of localizations. Co-localization is integrated into training by minimizing the color term of a conditional random field (CRF) loss over a sequence of frames/CAMs.
Extensive experiments on two challenging YouTube-Objects datasets of unconstrained videos show the merits of our CoLo-CAM method, and its robustness to long-term dependencies, leading to new state-of-the-art performance for WSVOL task.
Our code is publicly available: [github.com/sbelharbi/colo-cam](https://github.com/sbelharbi/colo-cam).


### Proposed Method

<br />

<p align="center">
  <a href="/material/colo-cam/proposal.png">
    <img src="{{ site.url }}/material/colo-cam/proposal.png"   alt="CoLo-CAM: Proposal" width="1000">
  </a>
</p>

<br />


### Results

<br />

<p align="center">
  <a href="/material/colo-cam/results.png">
    <img src="{{ site.url }}/material/colo-cam/results.png"   alt="CoLo-CAM: Results" width="1000">
  </a>
</p>

<br />

### Ablations


<br />

<p align="center">
  <a href="/material/colo-cam/multiple-ablations.png">
    <img src="{{ site.url }}/material/colo-cam/multiple-ablations.png"   alt="CoLo-CAM: Multiple ablations" width="1000">
  </a>
</p>

<br />

<p align="center">
  <a href="/material/colo-cam/ablation-terms.png">
    <img src="{{ site.url }}/material/colo-cam/ablation-terms.png"   alt="CoLo-CAM: Ablations terms" width="1000">
  </a>
</p>

<br />

<p align="center">
  <a href="/material/colo-cam/computation-time.png">
    <img src="{{ site.url }}/material/colo-cam/computation-time.png"   alt="CoLo-CAM: Computation time" width="1000">
  </a>
</p>

<br />

<p align="center">
  <a href="/material/colo-cam/backbone-and-sampling.png">
    <img src="{{ site.url }}/material/colo-cam/backbone-and-sampling.png"   alt="CoLo-CAM: Impact of backbones, and sampling techniques" width="1000">
  </a>
</p>

<br />


<p align="center">
  <a href="/material/colo-cam/stability-table.png">
    <img src="{{ site.url }}/material/colo-cam/stability-table.png"   alt="CoLo-CAM: Method stability - table" width="1000">
  </a>
</p>

<br />

<p align="center">
  <a href="/material/colo-cam/stability-plot.png">
    <img src="{{ site.url }}/material/colo-cam/stability-plot.png"   alt="CoLo-CAM: Method stability - plot" width="1000">
  </a>
</p>

<br />


### Visual Results

<br />

<p align="center">
  <a href="/material/colo-cam/visual-results.png">
    <img src="{{ site.url }}/material/colo-cam/visual-results.png" alt="CoLo-CAM: Visual results" width="1000">
  </a>
</p>

<br />

<br />

<p align="center">
  <a href="/material/colo-cam/visual-results-limitations.png">
    <img src="{{ site.url }}/material/colo-cam/visual-results-limitations.png"   alt="CoLo-CAM: Visual results - limitations" width="1000">
  </a>
</p>

<br />



### More Visual Demonstration

More demo: [here](https://github.com/sbelharbi/colo-cam/tree/main?tab=readme-ov-file#-results).

### Conclusion

This paper proposes a new CAM-based approach for WSVOL by introducing co-localization into a CAM-based method. Using pixel-color cue, our proposed CoLo-CAM method constrains CAM responses to be similar over visually similar pixels across all frames, achieving col-localization.
Our total training loss comprises per-frame and multi-frame terms optimized simultaneously via standard Stochastic Gradient Descent (SGD).
Empirical experiments showed that our produced CAMs become more discriminative. This translates into several advantageous properties: sharp, more complete, and less noisy activations localized more precisely around objects. Moreover, localizing small/large objects becomes more accurate. Additionally, our method is more robust to training with long time-dependency and leads to new state-of-the-art localization performance.

Despite its improvements, our method still holds some limitations. Our pixel pseudo-labels are less accurate since they come from a pretrained classifier. In particular, a major issue is the set of frames without object of interest in a video. In WSVOL, it is typically assumed that the video label transfers to each frame. However, in unconstrained videos, not all frames hold the labeled object. Therefore, the label is mistakenly transferred into empty frames. This furthermore allows the classifier to suggest relevant ROIs in such frames leading to more errors in training. One possible way to alleviate this issue is to leverage the per-class probabilities of the classifier to assess whether an object is present or not in a frame. Such likelihood can be exploited to discard frames or weight loss terms over them.

Another issue is related to inference that is performed frame by by frame without leveraging temporal information in a video. The negative impact of this can be observed over a sequence of predictions which are characterized by localization inconsistencies. This is illustrated by large shift in localization where the bounding box (and the CAM activation), moves abruptly from one location at a frame to completely different location at the next frame. Prediction without accounting for temporal dependencies can easily lead to such results. Future works may consider improving the inference procedure by leveraging spatiotemporal information at the expense of inference time.

We note that our method can use either CNN- or transformer-based architecture. The only requirement is that the architecture is able to perform both tasks: classification and localization.
A vision transformer-based (ViT) model can be employed as an encoder. A standard classification head can be used to perform classification task. A new localization head is required to replace our decoder to perform localization task. An architecture similar to the one  presented in [this work](https://arxiv.org/pdf/2310.06196) can be used in our work which is expected to yield better performance compared to CNN-based model as reported in their work. We leave this aspect for future work.



### Acknowledgments
This research was supported in part by the Canadian Institutes of Health Research, the Natural Sciences and Engineering Research Council of Canada, and the Digital Research Alliance of Canada.
