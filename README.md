# Video Recorder

A Python script using OpenCV and pandas to record videos from multiple UDP streams simultaneously.

## Features

- Records videos from multiple UDP streams in parallel using threading
- Adds timestamp information to each frame of the video
- Supports recording up to 30 frames per second (FPS)
- Outputs recorded videos as AVI files

## How to use

1. Install OpenCV and pandas by running `pip install opencv-python pandas`
2. Replace 'Video_List.xlsx' with the path to your Excel file containing the list of UDP URLs and corresponding SigIDs
3. Run the script using Python (e.g., `python VideoRecorder.ipynb`)

## Prerequisites

- OpenCV 4.x or later installed on your system
- pandas 1.x or later installed on your system
- Excel file with the required columns (IPAdd, SigID) and format

## Known issues

- The script does not handle errors in reading the Excel file. Make sure your file is well-formatted.
- The script does not handle network connection losses or video stream interruptions. It will continue running until all threads are completed.
