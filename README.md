# VideoBroadcaster

VideoBroadcaster is a Computer Vision-based video broadcasting application that functions as a virtual camera. It can be used in various video conferencing platforms like Google Meet, Zoom, and others to apply AI-based real-time processing to video streams.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Tools and Technologies](#tools-and-technologies)

## Introduction

VideoBroadcaster allows users to stream AI-enhanced video feeds using YOLO for object detection and PyVirtualCam for broadcasting the processed video as a virtual camera input. The system is built using FastAPI, making it efficient and easy to use.

## Features

- AI-powered object detection using YOLO.
- Virtual camera support for integration with Google Meet, Zoom, etc.
- FastAPI-based backend for real-time video processing.
- Fast document retrieval using FAISS vector store.
- Efficient video streaming using PyVirtualCam.

## Installation

1. Clone the repository to your local machine:

```
   git clone https://github.com/srijosh/VideoBroadcaster-using-Computer-Vision.git
```

2. Navigate to the project directory:

```
   cd VideoBroadcaster-using-Computer-Vision
```

3. Create a Conda Environment

```
   conda create -n broadcast python=3.11
   conda activate broadcast
```

4. Install the required dependencies:

```
   conda install pytorch==2.5.1 torchvision==0.20.1 pytorch-cuda=12.4 -c pytorch -c nvidia
   pip install -r requirements.txt
```

## Usage

1. Run the Video Broadcaster:

```
   uvicorn main:app --host 0.0.0.0 --port 8000

```

## Tools and Technologies

- FastAPI: For handling video streaming via a web service.
- YOLO: Used for real-time object detection.
- PyVirtualCam: Creates a virtual camera to broadcast processed frames.
- OpenCV: For image and video processing.
- Torch & NumPy: For AI model execution and data manipulation.
