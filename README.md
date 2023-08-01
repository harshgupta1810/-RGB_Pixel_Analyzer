# RGB Pixel Analyzer README.md

This README.md file provides an overview and explanation of the RGB Pixel Analyzer code created by Harsh Gupta (Desparete Enuf). The code is written in Python using the OpenCV and Pillow (PIL) libraries to capture and analyze RGB pixel values from a live video feed.

## Getting Started

### Prerequisites

To run the RGB Pixel Analyzer code, you need to have Python installed on your system. Additionally, you'll need to install the following Python packages:

- OpenCV (`cv2`): A popular computer vision library for image and video processing.
- Pillow (`PIL`): A library for working with images in Python.

You can install the required packages using the following command:

```bash
pip install opencv-python pillow
```

### Running the RGB Pixel Analyzer

1. Clone or download the repository containing the RGB Pixel Analyzer code.
2. Ensure you have the required prerequisites installed.
3. Run the Python script, and a window will appear showing the live video feed from your default camera.
4. To capture an image, press the 'c' key. A new window will appear displaying the captured image.
5. In the captured image window, double-click on any pixel, and a new window will display the RGB values of that pixel.
6. To quit the program, press the spacebar.

## Code Description

The RGB Pixel Analyzer code uses the OpenCV and Pillow libraries to perform the following tasks:

1. Capture Video: The code uses OpenCV's `cv2.VideoCapture` to access the default camera and capture live video frames.

2. Flip Image: The captured video frames are flipped horizontally using `cv2.flip` to correct the mirror effect.

3. Capture Image: When the 'c' key is pressed, the current frame is saved as an image ('1.png') using `cv2.imwrite`.

4. Convert to RGB: The saved image is then opened using Pillow's `Image.open`, and the RGB representation is obtained using `imge.convert('RGB')`.

5. Pixel Analysis: The code sets a mouse callback function (`PIX`) to the captured image window. When the user double-clicks on a pixel, the RGB values of that pixel are obtained, and a new window displays the RGB values in a colored box.

6. Quitting the Program: The program can be terminated by pressing the spacebar.

## Functionality

The RGB Pixel Analyzer allows you to:

- View the live video feed from your camera.
- Capture an image from the video feed.
- Analyze RGB pixel values by double-clicking on any pixel in the captured image.

## Acknowledgments

The RGB Pixel Analyzer code was created by Harsh Gupta (Desparete Enuf). It demonstrates basic video capturing and image processing using OpenCV and Pillow in Python. The code is a simple example of capturing live video and analyzing RGB pixel values.

## License

This project is open-source and licensed under the [MIT License](LICENSE). You are free to modify and distribute the code, but please provide proper attribution to the original creator, Harsh Gupta (Desparete Enuf).
