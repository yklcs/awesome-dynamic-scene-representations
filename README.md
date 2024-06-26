# Awesome Dynamic Scene Representations

A curated list of resources on dynamic scene representations.

## What are dynamic scene representations?

Dynamic scene representations (aka 4D scene representations) encode the time-variant properties of a three-dimensional scene.
They can be viewed as the 4D extension of 3D scene representations, adding time into 3D methods such as neural radiance fields (NeRFs) and 3D Gaussian splatting (3DGS).
This allows dynamic scene representations to synthesize and render novel views of scenes from sparse video inputs.

## Papers

### 2024

- **4D Gaussian Splatting for Real-Time Dynamic Scene Rendering** (Wu et al., CVPR 2024) \
  Applies position, rotation, and scaling deformation fields to a set of 3DGS Gaussians to represent dynamic scenes. \
  [Paper](https://arxiv.org/pdf/2310.08528v2.pdf) · [Code](https://github.com/hustvl/4DGaussians) · [Website](https://guanjunwu.github.io/4dgs/) - _4DGS (Wu et al.)_

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

- **Sync-NeRF: Generalizing Dynamic NeRFs
  to Unsynchronized Videos** (Kim et al., AAAI 2024) \
  Supports unsynchronized multiview video input for 4D NeRFs by introducing learnable time offsets. \
  [Paper](https://arxiv.org/pdf/2310.13356.pdf) · [Code](https://github.com/seoha-kim/Sync-NeRF) · [Website](https://seoha-kim.github.io/sync-nerf/) - _Sync-NeRF_

### 2023

- **HexPlane: A Fast Representation for Dynamic Scenes** (Cao et al., CVPR 2023) \
  Represents dynamic scenes with an explicit plane-based radiance field by decomposing the 4D spacetime grid into six planes. \
  [Paper](https://arxiv.org/pdf/2301.09632.pdf) · [Code](https://github.com/Caoang327/HexPlane) · [Website](https://caoang327.github.io/HexPlane/) - _HexPlane_

- **K-Planes: Explicit Radiance Fields in Space, Time, and Appearance** (Fridovich-Keil et al., CVPR 2023) \
  Represents static and dynamic scenes explicitly with radiance fields projected decomposed to six multiscale planes. \
  [Paper](https://arxiv.org/pdf/2301.10241.pdf) · [Code](https://github.com/sarafridov/K-Plane) · [Website](https://sarafridov.github.io/K-Planes/) - _K-Planes_

- **DynPoint: Dynamic Neural Point For View Synthesis** (Zhou et al., NeurIPS 2023) \
  Synthesized novels views from videos without encoding global scene representations by learning the inter-frame 3D correspondence. Neural points generated from estimated depth and optical flow between frames are used for rendering. \
  [Paper](https://arxiv.org/pdf/2310.18999.pdf) · [Code](https://github.com/kaichen-z/dynpoint) - _DynPoint_

- **Tensor4D: Efficient Neural 4D Decomposition for High-fidelity Dynamic Reconstruction and Rendering** (Shao et al., CVPR 2023) \
  Represents 4D radiance fields as nine planes, which are projections of three volumes, each of which is a projection of 4D spacetime. \
  [Paper](https://arxiv.org/pdf/2211.11610.pdf) · [Code](https://github.com/DSaurus/Tensor4D) · [Website](https://liuyebin.com/tensor4d/tensor4d.html) - _Tensor4D_

- **NeRFPlayer: A Streamable Dynamic Scene Representation with Decomposed Neural Radiance Fields** (Song et al., TVCG May 2023) \
  Separates scene into fields representing new, static, and deformed areas.
  Enables streaming with a sliding window along time over feature vectors. \
  [Paper](https://arxiv.org/pdf/2210.15947.pdf) · [Code](https://github.com/lsongx/nerfplayer-nerfstudio) · [Website](https://lsongx.github.io/projects/nerfplayer.html) - _NeRFPlayer_

- **Dynamic 3D Gaussians:
  Tracking by Persistent Dynamic View Synthesis** (Luiten et al., 3DV 2024) \
  Simultaneously synthesizes views and performs dense tracking on dynamic scenes by extending 3DGS Gaussians with motion and physics-based priors. \
  [Paper](https://arxiv.org/pdf/2308.09713.pdf) · [Code](https://github.com/JonathonLuiten/Dynamic3DGaussians) · [Website](https://dynamic3dgaussians.github.io) - _Dynamic 3D Gaussians_

- **Robust Dynamic Radiance Fields** (Liu et al., CVPR 2023) \
  Increases robustness by learning camera poses, making SfM inputs unnecessary.
  Uses separate static and dynamic radiance fields, where camera poses are optimized by the gradient flow from the static radiance field. \
  [Paper](https://arxiv.org/pdf/2301.02239.pdf) · [Code](https://github.com/facebookresearch/robust-dynrf) · [Website](https://robust-dynrf.github.io) - _RoDynRF_

### 2022

- **Neural 3D Video Synthesis from Multi-view Video** (Li et al., CVPR 2022) \
  Represents dynamic scenes with a NeRF taking time-dependent latent code inputs. \
  [Paper](https://arxiv.org/pdf/2103.02597.pdf) · [Website](https://neural-3d-video.github.io) - _DyNeRF_

- **Fast Dynamic Radiance Fields with Time-Aware Neural Voxels** (Fang et al., SIGGRAPH Asia 2022) \
  Represents dynamic scenes with time-aware neural voxels. 3D voxels store features which are queried with deformed coordinates and combined with temporal features. \
  [Paper](https://arxiv.org/pdf/2205.15285.pdf) · [Code](https://github.com/hustvl/TiNeuVox) · [Website](https://jaminfong.cn/tineuvox/) - _TiNeuVox_

### 2021

- **D-NeRF: Neural Radiance Fields for Dynamic Scenes** (Pumarola et al., CVPR 2021) \
  Extends NeRF to 4D with a deformation field network outputting displacement as a function of time and position. \
  [Paper](https://arxiv.org/pdf/2011.13961.pdf) · [Code](https://github.com/albertpumarola/D-NeRF) · [Website](https://www.albertpumarola.com/research/D-NeRF/index.html) - _D-NeRF_

## Datasets

### Synthetic

- **D-NeRF** \
  50-200 frames of dynamic subjects without backgrounds. Monocular with randomly changing camera poses every frame. \
  [Dropbox](https://www.dropbox.com/s/0bf6fl0ye2vz3vr/data.zip?dl=0)

  <img src="./dataset-samples/d-nerf.png" width="200" alt="d-nerf" />

### Real-world

- **DyNeRF** (Neural 3D Video Synthesis) \
  Indoor scenes with ~20 static multiview cameras. 2704×2028 resolution, <40s long @ 30fps. \
  [Github](https://github.com/facebookresearch/Neural_3D_Video)

  <img src="./dataset-samples/dynerf.png" width="200" alt="dynerf" />

- **Google Immersive** (Immersive Light Field Video with a Layered Mesh Representation) \
  Indoor and outdoor scenes with 46 static multiview cameras. 2560×1920 resolution, <30s long @ 30fps. \
  [Github](https://github.com/augmentedperception/deepview_video_dataset)

  <img src="./dataset-samples/google-immersive.png" width="200" alt="google-immersive" />

- **Nerfies** \
  Quasistatic and dynamic scenes captured casually with two smartphones, recording two monocular videos each for training and evaulation. Longest scene is ~300 frames long. \
  [Github](https://github.com/google/nerfies/releases/tag/0.1)

  <img src="./dataset-samples/nerfies.png" width="200" alt="nerfies" />

- **Technicolor** (Dataset and Pipeline for Multi-View Light-Field Video) \
  Scenes captured with 16 multiview cameras. 2048×1088 resolution. \
  [Website](https://www.interdigital.com/data_sets/light-field-dataset) (requires email for access)
