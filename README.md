# AutoPilot AI: Self-Driving Car Lane Detection and Steering Control

This project, **AutoPilot AI**, focuses on creating a self-driving car system with lane detection and steering angle calculation. Using computer vision and deep learning techniques, the system detects lanes and calculates the optimal steering angle to guide a car along a clear path. The repository includes pre-trained model files, code for processing images, and visualization of detected lanes and steering direction.

## Project Structure

```plaintext
NeuroDrive/
├── data/
├── main.ipynb                     # Jupyter Notebook with the code for lane detection and steering control
├── README.md                      # Project description and usage instructions
└── test_img.png                   # Sample image for testing lane detection and steering angle calculation
└── autoencoder_model.h5       # Pre-trained model for image processing (e.g., denoising or feature extraction)
```

## Features

- **Lane Detection**: The code processes road images to detect lane lines, which helps in keeping the car centered on the road.
- **Steering Angle Calculation**: Based on the detected lane positions, the code calculates the steering angle required to navigate through the lanes smoothly.
- **Model Integration**: Includes a pre-trained model (`autoencoder_model.h5`) which can be used for tasks like feature extraction or image preprocessing.

## Requirements

To run this project, you will need:
- `numpy`
- `opencv-python`
- `tensorflow`
- `matplotlib`

Install all dependencies with:
```bash
pip install -r requirements.txt
```

## Usage
Clone the repository:

```bash
git clone https://github.com/your-username/NeuroDrive.git
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
