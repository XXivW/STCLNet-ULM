<div align="center">

# STCLNet-ULM

### STCLNet-T: Efficient Spatiotemporal Localization<br>for Ultrasound Localization Microscopy

**Lightweight localization · Spatiotemporal modeling · High-throughput ULM**

[Overview](#overview) · [Public dataset](#public-dataset) · [Reconstruction gallery](#reconstruction-gallery) · [Repository structure](#repository-structure)

<br>

<a href="PALA_results/intensity/RatBrain.png">
  <img src="PALA_results/intensity/RatBrain.png" alt="Rat brain ULM intensity reconstruction" width="720" height="489">
</a>

*Microvascular reconstruction of the rat brain on the public PALA dataset.*

**4 samples &nbsp; / &nbsp; 3 visualization types &nbsp; / &nbsp; 12 reconstruction images**

</div>

---

## Overview

**STCLNet-T** is a lightweight three-input, three-output spatiotemporal localization network for high-throughput ultrasound localization microscopy (ULM).

This repository presents additional reconstruction results on the public **PALA dataset**, with complementary views of vascular structure and flow.


## Public dataset

The reconstructions shown below use the publicly available **PALA dataset**. PALA provides simulated and in vivo ultrasound data for ultrasound localization microscopy research.

| Resource | Description | Link |
| :--- | :--- | :--- |
| **PALA · GitHub** | MATLAB scripts and functions for the PALA benchmark, together with the LOTUS software. | https://github.com/AChavignon/PALA |
| **PALA · Zenodo** | Public simulated and in vivo datasets. | [Download datasets · DOI: 10.5281/zenodo.4343435](https://doi.org/10.5281/zenodo.4343435) |

We thank the PALA authors for making these resources publicly available. Please refer to the original repositories for dataset details, usage terms, and citation information.

## Reconstruction gallery

Explore each sample across the three visualization types. **Click any image to open the full-resolution PNG.** Color scales and annotations are retained as provided in the original images.

### Rat brain

<table>
  <thead>
    <tr>
      <th width="33%">Intensity</th>
      <th width="33%">Direction</th>
      <th width="33%">Velocity</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><a href="PALA_results/intensity/RatBrain.png"><img src="PALA_results/intensity/RatBrain.png" alt="Rat brain: intensity reconstruction" width="280" height="185"></a></td>
      <td align="center"><a href="PALA_results/direction/RatBrain.png"><img src="PALA_results/direction/RatBrain.png" alt="Rat brain: direction reconstruction" width="280"></a></td>
      <td align="center"><a href="PALA_results/velocity/RatBrain.png"><img src="PALA_results/velocity/RatBrain.png" alt="Rat brain: velocity reconstruction" width="280"></a></td>
    </tr>
  </tbody>
</table>

### Rat brain · bolus

<table>
  <thead>
    <tr>
      <th width="33%">Intensity</th>
      <th width="33%">Direction</th>
      <th width="33%">Velocity</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><a href="PALA_results/intensity/RatBrainBolus.png"><img src="PALA_results/intensity/RatBrainBolus.png" alt="Rat brain · bolus: intensity reconstruction" width="280"></a></td>
      <td align="center"><a href="PALA_results/direction/RatBrainBolus.png"><img src="PALA_results/direction/RatBrainBolus.png" alt="Rat brain · bolus: direction reconstruction" width="280"></a></td>
      <td align="center"><a href="PALA_results/velocity/RatBrainBolus.png"><img src="PALA_results/velocity/RatBrainBolus.png" alt="Rat brain · bolus: velocity reconstruction" width="280"></a></td>
    </tr>
  </tbody>
</table>

### Rat kidney

<table>
  <thead>
    <tr>
      <th width="33%">Intensity</th>
      <th width="33%">Direction</th>
      <th width="33%">Velocity</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><a href="PALA_results/intensity/RatKidney.png"><img src="PALA_results/intensity/RatKidney.png" alt="Rat kidney: intensity reconstruction" width="280" height="180"></a></td>
      <td align="center"><a href="PALA_results/direction/RatKidney.png"><img src="PALA_results/direction/RatKidney.png" alt="Rat kidney: direction reconstruction" width="280"></a></td>
      <td align="center"><a href="PALA_results/velocity/Kidney.png"><img src="PALA_results/velocity/Kidney.png" alt="Rat kidney: velocity reconstruction" width="280"></a></td>
    </tr>
  </tbody>
</table>

### Mouse tumor

<table>
  <thead>
    <tr>
      <th width="33%">Intensity</th>
      <th width="33%">Direction</th>
      <th width="33%">Velocity</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><a href="PALA_results/intensity/MouseTumor.png"><img src="PALA_results/intensity/MouseTumor.png" alt="Mouse tumor: intensity reconstruction" width="280"></a></td>
      <td align="center"><a href="PALA_results/direction/MouseTumor.png"><img src="PALA_results/direction/MouseTumor.png" alt="Mouse tumor: direction reconstruction" width="280"></a></td>
      <td align="center"><a href="PALA_results/velocity/MouseTumor.png"><img src="PALA_results/velocity/MouseTumor.png" alt="Mouse tumor: velocity reconstruction" width="280"></a></td>
    </tr>
  </tbody>
</table>

<details>
<summary><strong>Viewing notes</strong></summary>

- Open the original PNG to inspect fine vascular details and image annotations.
- Gallery images are scaled for display; source files retain their original resolution.
- Rat brain and rat kidney intensity previews use the aspect ratios of their corresponding direction images; click through to view the unmodified originals.
- Read velocity ranges from the annotations in each source image.
- The rat kidney velocity file is named `Kidney.png`; its intensity and direction files are named `RatKidney.png`.

</details>

## Repository structure

```text
STCLNet-ULM/
├── README.md
└── PALA_results/
    ├── intensity/
    │   ├── RatBrain.png
    │   ├── RatBrainBolus.png
    │   ├── RatKidney.png
    │   └── MouseTumor.png
    ├── direction/
    │   ├── RatBrain.png
    │   ├── RatBrainBolus.png
    │   ├── RatKidney.png
    │   └── MouseTumor.png
    └── velocity/
        ├── RatBrain.png
        ├── RatBrainBolus.png
        ├── Kidney.png
        └── MouseTumor.png
```

<!-- Add manuscript, citation, code, and video links here once their public locations are available. -->

---

<div align="center">

**STCLNet-T** · Ultrasound Localization Microscopy<br>
[Back to top](#stclnet-ulm)

</div>
