# License-Plate-Inspector
# License Plate Recognition Using Tesseract

This project focuses on detecting license plates in images using the Tesseract OCR (Optical Character Recognition) engine. The goal is to develop a system capable of accurately extracting license plate numbers from images for various applications such as traffic monitoring, parking management, and vehicle identification.

## Overview

License plate detection using Tesseract involves several steps, including image preprocessing, license plate localization, and character recognition. This repository provides resources and examples to help you understand and implement these steps effectively.

## Methodology

1. Image Preprocessing
   1. Grayscaling
   2. Blurring
   3. Thresholding
2. Extract Contours
3. Validate each contours based on aspect ratio and min height and width.Remove unnecessary contours.
5. Check No of white pixels(*In majority of license plate major part of license plate has white pixels when converted to Binary.*)
4. Adjust the angles of the plates if its not in horizontal, or inclined at some angle.
5. Use Tesseract to perform OCR on the probable plates and give the license plate.

## Results

![car_plate_1][0]
![car_plate_2][1]

## Usage

To use the license plate detection system:

1. Prepare input images containing vehicles with visible license plates.
2. Run the provided source code to perform license plate detection using Tesseract.
3. Evaluate the results and fine-tune the system as needed for improved accuracy.

## Dependencies

This project relies on the following dependencies:

- Tesseract OCR: A popular OCR engine for character recognition.
- OpenCV: An open-source computer vision library for image processing.
- Python: Programming language used for implementing the license plate detection system.

Make sure to install these dependencies before running the provided source code.

## Contributing

Contributions to this project are welcome! If you have ideas for improvements, new features, or bug fixes, feel free to open an issue or submit a pull request.

[0]: images/plate1.jpeg
[1]: images/plate2.jpeg
