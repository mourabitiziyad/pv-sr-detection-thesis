# PV-SR Detection Thesis

This repository contains the main thesis work on **Photovoltaic Super-Resolution Detection**. The project is organized into multiple interconnected repositories that handle different aspects of the research pipeline.

## 🏗️ Repository Structure

This thesis project is composed of four main repositories:

### 1. **Main Thesis Repository** (This Repo)
- Central coordination and documentation
- Thesis manuscript and research documentation
- Integration of all components
- Results compilation and analysis

### 2. **SR-Metrics** [`sr-metrics/`](./sr-metrics) 
📊 **Image Quality Assessment and Super-Resolution Metrics**
- Reference: https://github.com/mourabitiziyad/sr-metrics
- Comprehensive toolkit for evaluating super-resolution algorithms
- Implements both traditional (PSNR, SSIM) and literature-based metrics (BRISQUE, PIQE)
- Batch processing capabilities for algorithm comparison
- Multi-format support (TIFF, PNG) with geo-referencing

### 3. **Thesis Segmentation UI** [`thesis-segmentation-ui/`](./thesis-segmentation-ui)
🖥️ **Interactive Segmentation Interface**
- Reference: https://github.com/mourabitiziyad/thesis-segmentation-ui
- Web-based interface for photovoltaic panel segmentation
- Real-time visualization and customization tools
- Integration with machine learning models
- User-friendly interface for data labeling and validation
- **Segmentation Metrics**: IoU (Intersection over Union), Dice coefficient, pixel accuracy

### 4. **Download Satlas Map** [`download-satlas-map/`](./download-satlas-map)
🗺️ **Satellite Data Acquisition**
- Reference: https://github.com/mourabitiziyad/download-satlas-map
- Automated satellite imagery download utilities
- Integration with satellite data APIs
- Preprocessing pipeline for research datasets
- Geographic coordinate handling and mapping

## 🚀 Getting Started

### Prerequisites
- Python 3.7+
- Git
- Streamlit (for segmentation UI)
- Required Python packages (see individual repo requirements)

### Clone with Submodules
```bash
# Clone the main repository with all submodules
git clone --recursive https://github.com/mourabitiziyad/pv-sr-detection-thesis.git

# If already cloned, initialize submodules
git submodule update --init --recursive
```

## 📋 Research Components

### Data Acquisition
- **Source**: Satellite imagery via `download-satlas-map`
- **Processing**: Automated downloading and preprocessing
- **Coverage**: Geographic regions with photovoltaic installations

### Segmentation & Detection
- **Tool**: Interactive UI via `thesis-segmentation-ui`
- **Method**: Machine learning-based segmentation
- **Output**: Annotated datasets for training and validation

### Super-Resolution Enhancement
- **Algorithms**: ESRGAN, S2DR3, and custom implementations
- **Evaluation**: Comprehensive metrics via `sr-metrics`
- **Focus**: Enhancing satellite imagery resolution for better PV detection

### Quality Assessment
- **Traditional Metrics**: PSNR, SSIM, RMSE
- **Advanced Metrics**: BRISQUE, PIQE, Laplacian variance
- **Segmentation Metrics**: IoU, Dice coefficient, pixel accuracy
- **Analysis**: Statistical comparison and algorithm ranking

## 📊 Key Features

- **🔗 Integrated Pipeline**: Seamless workflow from data acquisition to analysis
- **📈 Comprehensive Metrics**: Multiple quality assessment approaches
- **🎯 Domain-Specific**: Tailored for photovoltaic detection applications
- **🛠️ Modular Design**: Independent components for flexibility
- **📱 User Interface**: Interactive tools for data annotation
- **🌍 Geospatial Support**: Geographic coordinate handling

## 📖 Documentation

Each submodule contains detailed documentation:
- [`sr-metrics/README.md`](./sr-metrics/README.md) - Metrics calculation and evaluation
- [`thesis-segmentation-ui/README.md`](./thesis-segmentation-ui/README.md) - UI setup and usage
- [`download-satlas-map/README.md`](./download-satlas-map/README.md) - Data acquisition tools

## 🤝 Contributing

This repository represents ongoing thesis research. For contributions or questions:
1. Check individual repository issues
2. Follow the established coding standards
3. Ensure compatibility across components

## 📚 Citation

If you use this work in your research, please cite:
```bibtex
@thesis{Mourabiti2025pvsr,
  title={Enhancing Photovoltaic Detection Using Generative AI for Super-Resolution Satellite Imagery},
  author={Ziyad Mourabiti},
  year={2025},
  school={Technical University of Munich}
}
```

## 🔧 Updating Submodules

To update all submodules to their latest commits:
```bash
git submodule update --remote
```

To update a specific submodule:
```bash
git submodule update --remote sr-metrics
```

---

**Note**: This repository uses Git submodules to maintain clean separation between different components while enabling integrated development. Each submodule tracks its respective repository and can be developed independently. 