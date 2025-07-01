<div align="center"> 
    <h1>
        Awesome SVG Generation ✨ 
    </h1>
</div>

A curated list of awesome papers, projects, and resources for Scalable Vector Graphics (SVG) generation. This collection focuses on the intersection of deep learning and vector graphics, highlighting recent advancements in generating structured, editable, and high-fidelity SVGs from various inputs.
The field is rapidly advancing, driven by innovations in large language models (LLMs), multimodal models (MLLMs), and diffusion-based techniques. This list aims to serve as a high-quality, up-to-date reference for researchers, developers, and designers working in this exciting domain.

---

## Contents

## 📖 Research Papers

This section provides a curated list of key research papers in SVG generation, categorized by their core methodology. The papers are sorted with the most recent publications first within each category.

### 🧠 Language & Multimodal Methods

These models frame SVG generation as a sequential or code generation task, leveraging architectures like Transformers and State Space Models. They excel at understanding structure, semantics, and utilizing SVG's full primitive set, often taking multimodal inputs like images and text.

| Name | Title | Date | Status | Code | Project Page |
| :--- | :--- | :--- | :--- | :--- | :--- |
| RLRF | [RLRF: Rendering-Aware Reinforcement Learning for Vector Graphics Generation](https://arxiv.org/abs/2505.20793) | 2025/05/30 | Preprint | - | - |
| LayerPeeler | [LayerPeeler: Autoregressive Peeling for Layer-wise Image Vectorization](https://arxiv.org/abs/2505.23740) | 2025/05/29 | Preprint | - | [Github Page](https://layerpeeler.github.io/) |
| Omni-SVG | [OmniSVG: A Unified Scalable Vector Graphics Generation Model](https://arxiv.org/abs/2504.06263) | 2025/04/28 | CVPR 2025 | [Github](https://github.com/OmniSVG/OmniSVG) | [Github Page](https://omnisvg.github.io/) |
| Chat2SVG | [Chat2SVG: Vector Graphics Generation with Large Language Models and Image Diffusion Models](https://arxiv.org/abs/2411.16602) | 2024/11/25 | CVPR 2025 | [Github](https://github.com/kingnobro/chat2svg) | [Github Page](https://chat2svg.github.io/) |
| StarVector | [StarVector: Generating Scalable Vector Graphics Code from Images and Text](https://arxiv.org/abs/2312.11556) | 2023/12/17 | CVPR 2025 | [Github](https://github.com/joanrod/star-vector) | [Github Page](https://starvector.github.io/) |
| IconShop | [IconShop: Text-Guided Vector Icon Synthesis with Autoregressive Transformers](https://arxiv.org/abs/2304.14400) | 2023/04/27 | SIGGRAPH Asia 2023 | [Github](https://github.com/kingnobro/IconShop) | [Github Page](https://icon-shop.github.io/) |

### 🎨 Differentiable Rendering & Diffusion-based Methods

These methods primarily optimize vector parameters (e.g., Bézier curve control points) by comparing a differentiably rendered raster image against a target. This target is often a real image or one synthesized by a powerful text-to-image diffusion model, leveraging its rich visual priors.

| Name | Title | Date | Status | Code | Project Page |
| :--- | :--- | :--- | :--- | :--- | :--- |
| SVGFusion | [Scalable Text-to-SVG Generation via Vector Space Diffusion](https://arxiv.org/abs/2412.10437) | 2024/12/11 | Preprint | [Github](https://github.com/ximinng/SVGFusion) | [Github Page](https://ximinng.github.io/SVGFusionProject/) |
| SVGDreamer | [SVGDreamer: Text Guided SVG Generation with Diffusion Model](https://arxiv.org/abs/2312.16476v4) | 2023/12/27 | CVPR 2024 | [Github](https://github.com/ximinng/SVGDreamer) | [Github Page](https://ximinng.github.io/SVGDreamer-project/) |
| DeepSVG | [A Hierarchical Generative Network for Vector Graphics Animation](https://arxiv.org/abs/2007.11301) | 2020/07/20 | NeurIPS 2020 | [Github](https://github.com/alexandre01/deepsvg) | [Project Page](https://alexandre01.github.io/deepsvg/) |

## 💾 Datasets & Benchmarks

A collection of key datasets and benchmarks crucial for training and evaluating SVG generation models.

### 📊 Datasets

| Name | Description | Size | Link |
| :--- | :--- | :--- | :--- |
| MMSVG-2M | A large-scale multimodal dataset with 2 million richly annotated SVG assets, including icons, illustrations, and characters. Introduced by OmniSVG. | 2M | [Hugging Face](https://huggingface.co/OmniSVG) |
| SVG-Stack | A large-scale dataset for Image-to-SVG and Text-to-SVG tasks, containing a diverse collection of vector graphics. | 2M | [Hugging Face](https://huggingface.co/datasets/starvector/svg-stack) |
| SVG-icons | A large-scale dataset of SVG icons used for training and evaluation in the DeepSVG paper. | 100k | [Github Link](https://github.com/alexandre01/deepsvg?tab=readme-ov-file#dataset)|
| FIGR-8-SVG | A dataset of simple, monochrome icons with corresponding textual descriptions, widely used for text-to-icon generation tasks in the IconShop paper. | 8k | [Github Link](https://github.com/kingnobro/IconShop?tab=readme-ov-file#dataset) |

### ⚖️ Benchmark

| Name | Description | Size | Link |
| :--- | :--- | :--- | :--- |
| SVG-Bench | A comprehensive benchmark suite from the StarVector authors, containing 10 datasets for 3 different tasks (Image-to-SVG, Text-to-SVG, Diagram Gen). | - | [Hugging Face](https://huggingface.co/collections/starvector/starvector-svg-datasets-svg-bench-67811204a76475be4dd66d09) |

## 🛠️ Tools & Resources

A curated list of essential software, libraries, and frameworks for working with SVGs, from manual editing to programmatic manipulation and optimization.

### ✒️ SVG Editors & Viewers

For creating, viewing, and manually editing vector graphics.

- [Inkscape](https://inkscape.org/): A powerful, free and open-source vector graphics editor that uses SVG as its native format.
- [Figma](https://www.figma.com/): A collaborative interface design tool with excellent support for vector editing and SVG export.
- [Online Editor](http://editor.method.ac/): A simple and clean open-source vector editor that runs in the browser.

### ⚙️ SVG Optimization

Tools for reducing file size by cleaning up redundant information and optimizing path data.

- [svgomg](https://jakearchibald.github.io/svgomg/): A web-based GUI to visually optimize SVG files, running SVGO under the hood.
- [svgo](https://svgo.dev/): A Node.js-based tool and library for optimizing SVG vector graphics files. The industry standard.
- [scour](https://github.com/scour-project/scour): A Python-based SVG optimizer that can also repair damaged files.

## 📦 Libraries & Frameworks

### 🐍 Python

For backend processing, data manipulation, and integration with deep learning models.

- [diffvg](https://github.com/BachiLi/diffvg): A differentiable rasterizer for vector graphics, enabling gradient-based optimization of SVG parameters. A core component in many optimization-based methods.
- [svglib](https://github.com/DataMarket/svglib): A library for reading SVG files and converting them into other formats (e.g., PDF, PNG) using the ReportLab toolkit.
- [svgwrite](https://github.com/mozman/svgwrite): A Python library to create SVG drawings programmatically. It's a drawing library, not a parser.
- [cairosvg](https://cairosvg.org/): A library to convert SVG files to various raster formats like PNG, PDF, and PostScript.
- [svgelements](https://github.com/meerk40t/svgelements): A robust Python library for parsing SVG files into a structured object model, supporting paths, shapes, and CSS styling.

### 🚢 Javascript

For web-based rendering, interaction, and animation.

- [d3js](https://d3js.org/): A powerful library for manipulating documents based on data. It brings data to life using HTML, SVG, and CSS.
- [snapsvg](http://snapsvg.io/): A JavaScript library that makes working with your SVG assets as easy as jQuery makes working with the DOM.
- [gsap](https://gsap.com/): A professional-grade animation library for the modern web, with robust support for SVG animation.
- [svgjs](https://svgjs.dev/): A lightweight library for manipulating and animating SVG with a clean, concise syntax.
- [Vivus.js](https://github.com/maxwellito/vivus): A lightweight, dependency-free JavaScript class that gives SVGs the appearance of being drawn.

## 🤝 Contributing

Contributions are welcome! If you have a suggestion for a paper, project, or resource to add, please feel free to open a pull request.
Please ensure your submission is high-quality and relevant to the topic of SVG generation. Follow the existing format and provide all necessary information (links, publication status, etc.).

## 📄 License

To the extent possible under law, the contributors have waived all copyright and related or neighboring rights to this work.
