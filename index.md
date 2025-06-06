---
layout: default
title: Quick Start
nav_order: 1
---

# Welcome to ITRI AI Hub Tutorials
##### update : 2025/01 by ITRI (EOSL-R3)

<br>ITRI AI Hub provides simple, fast, and commercialized Edge AI implementation solutions for enterprises and developers. Before selecting a system, we recommend evaluating which devices are best suited for your applications based on factors such as model type, computing power, memory, and energy efficiency. The diagram below summarizes the memory and computing power distribution of the devices we have selected, helping you intuitively compare them with a variety of Model Zoo options, open-source community models, or other custom models.

<div align="center">
<img src="docs/assets/images/pages/metric_of_all_devices.png" width="760"/>
</div>

## **Overview**

<div style="margin-left: 20px;">
<p>To support various types of AI tasks, users can pre-select base models from GitHub projects, open-source frameworks, or train their desired models using PyTorch or TensorFlow. These models rely on self-built workstations, servers, or cloud-hosted data centers during the design and development phases. 

In this regard, ITRI provides online resources such as <a href="https://azure.microsoft.com/en-us/products/machine-learning">Azure AI Foundry</a> and <a href="https://www.aita.org.tw/News/news_more?id=82a8da71e7cc4cf6acb657a789165822">AMD Instinct Cluster</a> to help you easily adapt and develop your products without incurring significant infrastructure maintenance costs. Additionally, you can quickly deploy your innovative applications by integrating pre-built tools and frameworks from the open-source community (e.g., YOLO, LLaMA, Whisper...) to obtain models.</p>
</div>

<strong>AI on Chips: Enabling the Future of AI Everywhere</strong>
<div style="margin-left: 20px;">
AI on Chips enables various types of electronic devices to efficiently execute AI models, offering unparalleled opportunities to realize the vision of AI Everywhere. To achieve this, integrating CPUs, GPUs, and NPUs into Chiplets plays a critical role, overcoming traditional performance and power consumption bottlenecks. For vendor-specific solutions and Taiwan's self-developed Silicon IP, ITRI provides a pilot production line for heterogeneous integration with small-volume, diverse packaging. This process fully covers the design, manufacturing, verification, and system integration testing of Chiplets, helping enterprises and academia quickly enter the market and build innovative applications on top of it.
</div><br>


<strong>How to Get Started with Chiplets?</strong>
<div style="margin-left: 20px;">
To ensure that models can run efficiently on embedded systems, AI developers must identify the hardware specifications and architecture of the chips. This is essential to fully leverage the application performance of advanced AI chips. You can find more information on other pages of this document:
<ul>
    <li><a href="https://r300-ai.github.io/ITRI-AI-Hub/">Raspberry Pi Board</a></li>
    <li><a href="https://r300-ai.github.io/ITRI-AI-Hub/docs/genio-evk.html">Genio Board</a></li>
    <li><a href="https://r300-ai.github.io/ITRI-AI-Hub/docs/ryzen.html">Ryzen AI Board</a></li>
    <li><a href="https://r300-ai.github.io/ITRI-AI-Hub/">Jetson Board</a></li>
    <li><a href="https://r300-ai.github.io/ITRI-AI-Hub/">WiseEye Visual AI Accelerator (MCU)</a></li>
    <li><a href="https://r300-ai.github.io/ITRI-AI-Hub/">Hailo Visual AI Accelerator (MCU)</a></li>
</ul>
</div>

## **Development Flow**

At AI Hub, we provide comprehensive guides for various types of Chiplets, including system configuration methods and model deployment tutorials.

1. First, obtain an Evaluation Kit from an authorized retailer or distributor. Then, follow the official documentation to configure the installation environment and operating system according to your requirements.
2. The Developer Zone provides concise notes and shared resources to assist with the setup process.
3. Next, utilize the benchmark data available in the [Model Zoo](https://github.com/R300-AI/ITRI-AI-Hub/tree/main/Model-Zoo) to evaluate the performance of each chip and determine its suitability for your application needs.
4. Finally, use the provided testing tools to assess your model's performance on different processing units across various Chiplets, to gain detailed insights into AI acceleration techniques and optimization strategies.

> [**NOTE**] It is essential to recognize that each chip vendor operates within its own distinct hardware and software ecosystem. Nevertheless, the following framework is widely adopted by most AI developers, providing a systematic approach to efficiently evaluate and select the most suitable chip:
>
> <table>
>   <thead>
>     <tr>
>       <th style="width: 10%;">Processing Unit</th>
>       <th style="width: 5%;">Memory Usage</th>
>       <th style="width: 12%;">Supported Computing Operators</th>
>       <th style="width: 12%;">Ideal Use Case</th>
>       <th style="width: 61%;">Notes</th>
>     </tr>
>   </thead>
>   <tbody>
>     <tr>
>       <td>CPU</td>
>       <td>Medium</td>
>       <td>General-purpose logic</td>
>       <td>Control flow and non-parallel ML tasks</td>
>       <td>Executes general-purpose code directly. The performance of ML models can be further enhanced using vendor-optimized libraries (e.g., OpenVINO, ZenDNN, Kleidi AI...).</td>
>     </tr>
>     <tr>
>       <td>GPU</td>
>       <td>High</td>
>       <td>Graphics rendering and parallel computing</td>
>       <td>Matrix multiplication and neural network inference</td>
>       <td>Requires the installation of appropriate graphics drivers (e.g., CUDA for NVIDIA GPUs, ROCm for AMD GPUs) and the use of related execution provider (e.g., TensorRT) to utilize GPU computing resources.</td>
>     </tr>
>     <tr>
>       <td>NPU</td>
>       <td>Low</td>
>       <td>Specialized AI operators</td>
>       <td>Low-power, high-efficiency neural network inference</td>
>       <td>Requires the installation of drivers and execution providers. Additionally, vendor-provided quantization tools are often necessary to compile models, as these tools map a subset of valid operators to NPU computing resources for optimized performance.</td>
>     </tr>
>   </tbody>
> </table>

## **Open-Source Community Highlights**
### Data Preparation
* [Label Studio: Open Source Data Labeling](https://labelstud.io/)
* [Albumentations: fast and flexible image augmentations](https://albumentations.ai/)

### Training Model

### Quantization and Deployment
* [Computer Vision Deployment on Genio DLAs Using Ultralytics Pre-Trained YOLOs]()
