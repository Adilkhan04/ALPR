# ALPR
 Powerful ALPR with YOLOv8, ESRGAN &amp; EasyOCR! ⚡️ Detect &amp; read license plates in images/videos. ✨ High accuracy, real-time performance, flexible &amp; open-source. Optimized for accuracy and speed. Detect and read plates effectively!.  Code, docs, contribute! #ALPR #YOLOv8 #ESRGAN #EasyOCR 


Automatic License Plate Recognition (ALPR) System with YOLOv8, ESRGAN, and EasyOCR
## Overview:

This repository presents a real-time, highly accurate ALPR system trained on a combination of YOLOv8, ESRGAN, and EasyOCR models. It can detect and recognize license plates of various shapes and sizes, even in challenging environments like low-light conditions.
## Methodology:
Our ALPR solution employs a combination of custom-trained YOLOv8, EasyOCR, and pre-trained ESRGAN models. The methodology involves:

1. **Training the YOLOv8 algorithm** to detect license plates in images.
2. Using **ESRGAN** to enhance the quality of low-resolution images, resulting in high-quality output.
3. Sharing this output with YOLOv8, which detects the license plate in images by mapping the license plate coordinates.
4. Transferring the output of YOLOv8 to **EasyOCR**, which detects the characters in the license plate and finally displays the output.
## Key Features:

Real-time performance: Handles video streams and images with minimal latency.
High accuracy: Achieves 97% F1 score and 98.5% mean average precision on diverse datasets.
Versatility: Operates in complex environments like low-light conditions.
Open-source and adaptable: The code is readily available for customization and improvement.
System Architecture:
![Screenshot 2023-10-27 110147](https://github.com/Adilkhan04/ALPR/assets/79263426/9bf200c3-a507-425f-a7ae-8a4f221b5b8f)

YOLOv8 Detection: A custom-trained YOLOv8 model identifies license plates within images or video frames.
![Screenshot 2023-07-26 122139](https://github.com/Adilkhan04/ALPR/assets/79263426/4a9a394d-98da-4c9f-9629-297e4b49cdf1)
ESRGAN Super-Resolution: For blurry or low-resolution images, ESRGAN enhances the quality before feeding it back to YOLOv8 for improved accuracy.
![image](https://github.com/Adilkhan04/ALPR/assets/79263426/757b3ea6-2c48-48bd-8d7f-2e719334de49)
![lp_cropped](https://github.com/Adilkhan04/ALPR/assets/79263426/bc72725a-afea-432a-a981-dc65bf0b228f)
![lp](https://github.com/Adilkhan04/ALPR/assets/79263426/2ebb07a9-c9e9-491b-ab25-93ba7eae8416)
![lpr](https://github.com/Adilkhan04/ALPR/assets/79263426/25658d00-1889-4b87-92bb-180737843671)

EasyOCR Recognition: Based on YOLOv8's output, EasyOCR extracts and recognizes the characters on the license plate.


https://github.com/Adilkhan04/ALPR/assets/79263426/c39a7ef8-643c-49e0-a5dc-ac411d0ed72c

## Benefits:

Enhanced security and surveillance: Track vehicles, enforce traffic regulations, and improve security systems.
Automated data collection: Extract license plate information for research, toll booths, or vehicle access control.
Streamlined workflows: Eliminate manual data entry and human errors associated with license plate reading.
Getting Started:

Clone the repository and install the required dependencies.
Download the pre-trained models for YOLOv8 and ESRGAN, and import the EasyOCR library.
train the YOLOv8 model, you can get the dataset from roboflow.com
make sure that yolo is version 8.0.0 otherwise train the YOLOv8 from Ultralytics official repository in GitHub
and run the model with integrated YOLOv8 and ESRGAN

## Future work:
In the future, there is potential to enhance ALPR systems by incorporating more parameters such as driver facial recognition and vehicle speed. Additionally, it would be beneficial to create a user-friendly interface for the system.
one can also custom-train an ESRGAN instead of a pre-trained model or use a more advanced super-resolution model for improving license plate detection quality but remember it should be able to detect in Real-time
