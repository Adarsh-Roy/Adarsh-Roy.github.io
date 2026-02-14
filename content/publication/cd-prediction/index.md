---
title: "Car Drag Coefficient Prediction from 3D Point Clouds Using a Slice-Based Surrogate Model"
authors:
- admin
- utkarsh
- absaar
date: "2025-09-21T00:00:00Z"

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["conference-paper"]

# Publication name and optional abbreviated publication name.
publication: "Springer Nature Lecture Notes on Computer Science"
publication_short: "SN LNCS"

abstract: The automotive industry’s pursuit of enhanced fuel economy and performance necessitates efficient aerodynamic design. However, traditional evaluation methods such as computational fluid dynamics(CFD) and wind tunnel testing are resource intensive, hindering rapid iteration in the early design stages. Machine learning-based surrogate models offer a promising alternative, yet many existing approaches suffer from high computational complexity, limited interpretability, or insufficient accuracy for detailed geometric inputs. This paper introduces a novel lightweight surrogate model for the prediction of the aerodynamic drag coefficient (Cd) based on a sequential slice-wise processing of the geometry of the 3D vehicle. Inspired by medical imaging, 3D point clouds of vehicles are decomposed into an ordered sequence of 2D cross-sectional slices along the stream-wise axis. Each slice is encoded by a lightweight PointNet2D module,and the sequence of slice embeddings is processed by a bidirectional LSTM to capture longitudinal geometric evolution. The model, trained and evaluated on the DrivAerNet++ dataset, achieves a high coefficient of determination (R2 > 0.9528) and a low mean absolute error (MAE ≈ 6.046 × 10−3) in Cd prediction. With an inference time of approximately 0.025 seconds per sample on a consumer-grade GPU, our approach provides fast, accurate, and interpretable aerody- namic feedback, facilitating more agile and informed automotive design exploration.

# Summary. An optional shortened abstract.
summary: A lightweight slice-based model predicts vehicle drag (Cd) directly from 3D point clouds with high accuracy and fast inference.

tags:
- Deep Learning
- Automotive Aerodynamics

featured: true

# hugoblox:
#   ids:
#     arxiv: 1512.04133v1

links:
# - type: preprint
#   provider: arxiv
#   id: 1512.04133v1
- type: code
  url: https://github.com/Adarsh-Roy/cd_prediction
# - type: slides
#   url: https://www.slideshare.net/
- type: dataset
  url: https://paddlescience.readthedocs.io/en/latest/zh/examples/drivaernetplusplus/
# - type: poster
#   url: "#"
- type: source
  url: https://doi.org/10.1007/978-3-032-11442-6_5
# - type: video
#   url: https://youtube.com
- type: custom
  label: Live Demo
  url: https://cdprediction.streamlit.app/

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
