# Video Magnify Upscale - ComfyUI Workflow

**High-quality video upscaling workflow for Sora 2 and other AI-generated videos using WAN model in ComfyUI**

![Example 1](01.gif) ![Example 2](02.gif) ![Example 3](03.gif)

![Example 4](04.gif) ![Example 5](05.gif)

## 📖 Overview

This repository provides a ComfyUI workflow designed specifically for upscaling and enhancing AI-generated videos from Sora 2 (OpenAI's latest video generation model) and other sources. The workflow uses a progressive magnification technique combined with the WAN (Waifu Anime Network) model to achieve high-quality results.

### Why This Workflow?

Sora 2 and similar AI video generation models can sometimes produce videos with suboptimal quality or resolution. This workflow addresses this by:

- **Progressive Magnification**: Uses a multi-stage upscaling approach that progressively increases resolution
- **LLM-Assisted Enhancement**: Leverages large language models to guide the upscaling process
- **Quality Over Speed**: Prioritizes output quality through careful resolution management

### The Approach

The workflow implements a unique strategy:
1. **Downscale First**: Input video is initially downscaled to ~360p (reduces artifacts and normalizes quality)
2. **Progressive Upscale**: Uses magnification passes to gradually increase resolution
3. **Final Output**: Produces crisp 720p output with enhanced details

This counter-intuitive "downscale then upscale" approach helps eliminate compression artifacts and ensures consistent quality throughout the upscaling process.

## 🎯 Credits

**Important:** This workflow is built upon the excellent work by [@cseti007](https://github.com/cseti007).

- **Original Workflow Creator**: [@cseti007](https://github.com/cseti007)
- **Original Workflows Repository**: [ComfyUI-Workflows](https://github.com/cseti007/ComfyUI-Workflows)

Please visit cseti007's repository for more amazing ComfyUI workflows and upscaling techniques!

## 🚀 Getting Started

### Prerequisites

- **ComfyUI** installed and configured
- **WAN Model** (Waifu Anime Network) - Download and place in your ComfyUI models directory
- **Hardware Requirements**:
  - **Recommended**: NVIDIA RTX 6000 Pro or equivalent
  - **Minimum**: 12GB+ VRAM for stable operation
  - Adequate system RAM (16GB+ recommended)

### Installation

1. Clone this repository:
```bash
git clone https://github.com/lovisdotio/workflow-magnify-upscale-video-comfyui-lovis.git
cd workflow-magnify-upscale-video-comfyui-lovis
```

2. Load the workflow in ComfyUI:
   - Open ComfyUI
   - Click "Load" and select `workflow-upscale-video-wan-lovis-v1.json`
   - Ensure all required custom nodes are installed

3. Place your input video in an accessible location

4. Configure the workflow parameters as needed

## 💡 Usage

1. **Load the Workflow**: Import `workflow-upscale-video-wan-lovis-v1.json` into ComfyUI
2. **Set Input Video**: Point the input node to your source video (works great with Sora 2 outputs!)
3. **Adjust Settings** (optional):
   - Frame rate
   - Resolution targets
   - Upscaling strength
4. **Run the Workflow**: Execute and wait for processing to complete
5. **Retrieve Output**: Your upscaled video will be saved in the ComfyUI output directory

### Tips for Best Results

- **Sora 2 Videos**: This workflow was optimized for Sora 2 output, but works with any video
- **Resolution**: Input videos around 360-480p tend to work best
- **Frame Rate**: Maintain original frame rate for temporal consistency
- **Batch Processing**: Process videos in batches if you have multiple files

## 📊 Examples

All example GIFs in this repository demonstrate before/after comparisons of the upscaling process. These showcase the workflow's ability to:
- Enhance fine details
- Reduce compression artifacts
- Improve overall visual clarity
- Maintain temporal consistency across frames

## 🛠️ Technical Details

The workflow leverages:
- **WAN Model**: For intelligent upscaling with content awareness
- **Progressive Magnification**: Multi-pass approach prevents quality degradation
- **LLM Integration**: Helps guide enhancement decisions based on content analysis
- **ComfyUI Nodes**: Modular design allows for easy customization

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

## 📝 License

This project is open source and available under the MIT License.

## 🙏 Acknowledgments

- **[@cseti007](https://github.com/cseti007)** - Original workflow creator and inspiration
- **ComfyUI Community** - For the amazing framework and ecosystem
- **WAN Model Developers** - For the powerful upscaling model
- **Sora 2 Team** - For pushing the boundaries of AI video generation

## 📧 Contact

For questions or suggestions, feel free to open an issue or reach out!

---

**Star ⭐ this repository if you find it useful!**

