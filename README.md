# NeuroDrive
# NeuroDrive: Self-Driving Car Lane Detection and Steering Control

**NeuroDrive** is an AI-powered self-driving car system that focuses on lane detection and steering angle calculation. Using computer vision and deep learning techniques, NeuroDrive identifies lanes on the road and calculates the optimal steering angle required to navigate smoothly. This repository includes code for image processing, a pre-trained model, and visualizations to guide a car along a clear path.

## Project Structure


```plaintext
NeuroDrive/
├── data/
├── main.ipynb                     # Jupyter Notebook with the code for lane detection and steering control
├── README.md                      # Project description and usage instructions
└── test_img.png                   # Sample image for testing lane detection and steering angle calculation
└── autoencoder_model.h5           # Pre-trained model for image processing (e.g., denoising or feature extraction)
```

## Features

- **Lane Detection**: Detects and highlights lane lines on road images to keep the car centered.
- **Steering Angle Calculation**: Calculates the optimal steering angle based on detected lane positions, helping to ensure safe and accurate navigation.
- **Model Integration**: Includes a pre-trained autoencoder model (`autoencoder_model.h5`) for tasks like feature extraction and preprocessing to improve image quality and detection accuracy.

## Requirements

The project requires Python and the following libraries:
- `numpy`
- `opencv-python`
- `tensorflow`
- `matplotlib`

You can install all required libraries with the following command:
```bash
pip install -r requirements.txt
```
Usage
Clone the repository:

```bash
git clone https://github.com/prachidave13/NeuroDrive
```
```bash
cd NeuroDrive
```

### Open the Notebook

Launch `main.ipynb` in Jupyter Notebook or any compatible IDE (e.g., Jupyter Lab, Google Colab).

### Run the Lane Detection Pipeline

1. **Load `test_img.png`** or any road image you would like to test.
2. Execute the cells in the notebook to process the image, detect lanes, and calculate the required steering angle.

### Visualize Results

The notebook includes visualization code to display detected lanes and the calculated steering angle directly on the road image, making it easier to interpret the system's decisions.

### Example

- **Input**: `test_img.png` - a sample road image used for testing.
- **Output**: Visual output showing detected lanes overlaid on the road and an arrow indicating the suggested steering angle.

### Future Work

- **Enhanced Lane Detection**: Add functionality to handle varying lighting and weather conditions for more robust lane detection.
- **Real-Time Controls**: Integrate with real-time control systems for potential applications in virtual simulations or physical models.

