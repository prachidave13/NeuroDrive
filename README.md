### Project Description: Self-Driving Vehicle: Lane Detection and Steering Angle Calculation

**Objective:**
My goal for this project is to develop an autonomous lane detection system for self-driving vehicles using deep learning and computer vision. The system will detect lane markings from dashboard camera images and calculate the appropriate steering angle to keep the vehicle centered within its lane.

**Steps:**

#### Auto-Encoder Model for Lane Detection:

**Build and Train the Model:**
I built and trained an auto-encoder neural network to identify lane markings in images. The model uses convolutional layers for feature extraction and up-sampling layers for image reconstruction, highlighting lane lines.

**Dataset:**
I got a dataset of road images, preprocessed them, and used them to train the auto-encoder.

#### Lane Detection Using OpenCV:

**Preprocessing:**
I converted images to grayscale and applied Gaussian blur to reduce noise.

**Edge Detection:**
Using Canny edge detection, I highlighted edges in the images.

**Region of Interest (ROI):**
I applied a mask to focus on the relevant portion of the image where lanes are likely to appear.

**Hough Transform:**
I used the Hough Transform technique to detect lines within the ROI, representing the lane markings.

#### Steering Angle Calculation:

**Lane Center Calculation:**
I used the detected lanes to determine the center of the lane.

**Angle Determination:**
I calculated the vehicle’s deviation from the lane center and computed the corresponding steering angle to guide the vehicle back to the center.

#### Integration and Testing:

**Pipeline Implementation:**
I created an integrated pipeline to process images, detect lanes, and calculate the steering angle in real-time.

**Testing:**
I tested the pipeline on various images to ensure the system’s robustness and accuracy.

**Outcome:**
The system successfully identifies lane markings and calculates the necessary steering adjustments, demonstrating a foundational step towards fully autonomous driving capabilities. This project showcases the integration of deep learning and computer vision to solve a practical problem in autonomous vehicles, providing a stepping stone for further advancements in self-driving technology.
