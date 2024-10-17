# Playing Card Detection for Blackjack

This project implements a playing card detection system using TensorFlow and OpenCV, specifically designed for the game of Blackjack. The goal is to accurately identify playing cards in real-time, determine their values, and facilitate a game experience where users can play against a virtual dealer.

## Table of Contents

- Features
- Installation
- Usage
- Training the Model
- How It Works

## Features

- **Real-Time Image Capture**: Collect images from your webcam and save them in organized directories.
- **Customizable Labels**: Define your own labels for image categorization.
- **User-Friendly Interface**: Easy-to-use commands for taking screenshots and organizing images.
- **Annotation Tool**: Integration with the LabelImg tool for labeling images, preparing datasets for model training.
- **Real-Time Card Detection**: Detect playing cards using a custom TensorFlow object detection model.
- **Card Value Calculation**: Implement Blackjack rules, including the handling of Aces.
- **Live Video Feed Processing**: Display detected cards and their values in real-time.
- **Game Condition Handling**: Manage game conditions such as Blackjack and BUST scenarios.

## Installation

To set up the project, follow these steps:

1. **Install Required Libraries**: Make sure you have Python and the necessary libraries installed.
2. **Set Up LabelImg**: Clone the LabelImg repository and set it up for annotating images.

## Usage

### Step 1: Collect Images

Run the provided script to collect images from your webcam based on specific labels for the playing cards:

1. Define your labels (e.g., AS, KS, 2S, etc.).
2. Use OpenCV to capture images and save them in organized directories.

### Step 2: Take Screenshots

You can also use the script to take screenshots of the playing cards while running the webcam feed. The key bindings allow you to label the images as you capture them.

### Step 3: Annotate Images with LabelImg

After collecting images, use the LabelImg tool to annotate them. This is essential for training your model later.

### Step 4: Training the Model

To train your custom object detection model with the collected and annotated images, you will need to follow the TensorFlow object detection API guidelines. Ensure you have the required dependencies and data preparation steps completed.

## How It Works

1. **Image Collection**: The tool captures images of playing cards from the webcam based on user-defined labels.
2. **Image Saving**: Images are saved in a structured format using a unique identifier to ensure no duplicates.
3. **Real-Time Detection**: The system processes a live video feed to detect and classify playing cards, providing immediate feedback on the game state.
