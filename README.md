# Bee Detection Project

## Overview

This project is dedicated to detecting bees in images or videos using computer vision techniques and machine learning models. The aim is to support ecological research, monitor bee populations, and assist in understanding their behaviors and habitats.
We using dataset from  VnPollenBee Dataset. It contains more than 2000 imagesconsisting of 1,758 pollen bearing and 59,068 non-pollen bearing bees.

## Features

- **Image Detection:** Identify and locate bees in static images.
- **Video Detection:** Track bee movements in real-time or pre-recorded videos.
- **Analytics Dashboard:** View insights like bee count, movement patterns, and detection confidence levels.
- **Customizable Models:** Fine-tune detection models for specific environments or bee species.

## Project Structure

```
bee-detection/
|-- data/                # Dataset storage (images/videos)
|-- models/              # Pretrained models and checkpoints
|-- src/                 # Source code for the project
|   |-- detection/       # Bee detection logic
|   |-- utils/           # Helper functions
|   |-- visualization/   # Code for plotting and displaying results
|-- notebooks/           # Jupyter notebooks for experiments
|-- tests/               # Unit tests for the codebase
|-- README.md            # Project documentation (this file)
|-- requirements.txt     # Python dependencies
|-- setup.py             # Installation script
```

## Getting Started

### Prerequisites

- **Python 3.8+**
- Recommended libraries:
  - OpenCV
  - TensorFlow or PyTorch
  - NumPy
  - Matplotlib

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/bee-detection.git
   cd bee-detection
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Download the dataset and place it in the `data/` folder.

### Running the Project

#### Detect Bees in an Image

```bash
python src/detection/detect_image.py --image_path data/images/sample.jpg --output_path results/output.jpg
```

#### Detect Bees in a Video

```bash
python src/detection/detect_video.py --video_path data/videos/sample.mp4 --output_path results/output.mp4
```

#### Training a Model

To train a custom model, use:

```bash
python src/train.py --data_path data/dataset --epochs 50 --output_model models/custom_model.pth
```

## Datasets

The project supports public datasets or custom datasets for training and testing. Ensure your dataset follows the format below:

```
data/
|-- images/
|   |-- img1.jpg
|   |-- img2.jpg
|-- labels/
    |-- img1.xml (or .json for annotations)
    |-- img2.xml
```

## Results

- Provide a folder `results/` to store output images and videos.
- Use `src/visualization/plot_results.py` to visualize detection metrics like accuracy and precision.

## Contributing

We welcome contributions to improve this project! Please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature.
3. Commit and push your changes.
4. Submit a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments

- Open-source libraries: TensorFlow, PyTorch, OpenCV.
- Datasets: Include a note on public datasets used (if applicable).

---

Feel free to reach out for questions or collaborations!

