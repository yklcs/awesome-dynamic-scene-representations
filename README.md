# Awesome Dynamic Scene Representations

A curated list of resources on dynamic scene representations.

## What are dynamic scene representations?

Dynamic scene representations (aka 4D scene representations) encode the time-variant properties of a three-dimensional scene.
They can be viewed as the 4D extension of 3D scene representations, adding time into 3D methods such as neural radiance fields (NeRFs) and 3D Gaussian splatting (3DGS).
This allows dynamic scene representations to synthesize and render novel views of scenes from sparse video inputs.

## Papers

### 2024

The following papers extend 3D Gaussian splatting.

- **4D Gaussian Splatting for Real-Time Dynamic Scene Rendering** (Wu et al., CVPR 2024) \
  Applies position, rotation, and scaling deformation fields to a set of 3DGS Gaussians to represent dynamic scenes. \
  [Paper](https://arxiv.org/pdf/2310.08528v2.pdf) · [Code](https://github.com/hustvl/4DGaussians) · [Website](https://guanjunwu.github.io/4dgs/) - _4DGS (Wu et al.)_

Plane-based explicit method.

- **Real-time Photorealistic Dynamic Scene Representation and Rendering with 4D Gaussian Splatting** (Yang et al., ICLR 2024) \
  Uses learned 4D Gaussians and time-dependent color to represent dynamic scenes. \
  [Paper](https://arxiv.org/pdf/2310.10642.pdf) · [Code](https://github.com/fudan-zvg/4d-gaussian-splatting) · [Website](https://fudan-zvg.github.io/4d-gaussian-splatting/) - _4DGS (Yang et al.)_

- **Spacetime Gaussian Feature Splatting for Real-Time Dynamic View Synthesis** (Li et al., CVPR 2024) \
  Extends 3DGS to 4D with polynomial motion, time-dependent opacity, and temporal features. \
  [Paper](https://arxiv.org/pdf/2312.16812.pdf) · [Code](https://github.com/oppo-us-research/SpacetimeGaussians) · [Website](https://oppo-us-research.github.io/SpacetimeGaussians-website/) - _Spacetime Gaussians_

- **DaReNeRF: Direction-aware Representation for Dynamic Scenes** (Lou et al., CVPR 2024) \
  Improves plane-based models by applying dual-tree complex wavelet transforms to obtain a direction-aware representation. \
  [Paper](https://arxiv.org/pdf/2403.02265.pdf) · [Video](https://www.youtube.com/watch?v=hYQsl6Rbxn4) - _DaReNeRF_

- **Sparse-Controlled Gaussian Splatting for Editable Dynamic Scenes** (Huang et al., CVPR 2024) \
  Uses sparse control points to guide the deformation of 3DGS Gaussians, allowing for an editable dynamic representation. \
  [Paper](https://arxiv.org/pdf/2312.14937.pdf) · [Code](https://github.com/yihua7/SC-GS) · [Website](https://yihua7.github.io/SC-GS-web/) - _SC-GS_

## Datasets
