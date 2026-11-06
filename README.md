# MUTED
### A Real-Time Hand Gesture-Driven Game for Evaluating the Necessity of Temporal Modeling

**MUTED** is a real-time hand gesture-driven game developed by **CSA1**, led by **Angelito Flordeliza**, as part of a thesis project.

The project explores a central research question:

> **Is temporal modeling necessary for accurate and responsive hand gesture-based game control?**

MUTED serves as an experimental environment for investigating whether incorporating temporal information through recurrent architectures improves hand gesture recognition and control compared to a conventional CNN-based approach.

Rather than relying on traditional keyboard or controller inputs, players interact with the game using hand gestures captured through a camera. The system recognizes and translates physical hand movements into real-time in-game actions.

---

## Research Objective

The primary objective of MUTED is to evaluate the necessity and effectiveness of temporal modeling in hand gesture recognition for real-time interactive applications.

To investigate this, the project implements and compares two custom deep learning approaches:

- **CNN Baseline:** A convolutional neural network that performs hand gesture classification based on individual input frames.
- **CNN + GRU:** A hybrid architecture combining convolutional feature extraction with a Gated Recurrent Unit (GRU) to capture temporal dependencies across sequences of hand gestures.

By comparing these two approaches within the same game environment, the study aims to determine whether temporal information provides meaningful improvements in gesture recognition and real-time game control.

## Key Features

- **Real-Time Hand Gesture Control** – Control game interactions using camera-detected hand gestures.
- **Computer Vision Integration** – Uses MediaPipe for hand landmark detection and tracking.
- **Custom Deep Learning Models** – Implements a CNN baseline and a CNN+GRU architecture.
- **Temporal Modeling Evaluation** – Provides an experimental setup for comparing frame-based and sequence-based gesture recognition.
- **Real-Time Performance** – Designed around a 30 FPS target for responsive gameplay.
- **Custom Dataset** – Models trained using a self-collected dataset containing approximately 5,600 samples.
- **Local Model Training** – Model development and training were conducted on the developer's own machine.

## Technology Stack

| Technology | Purpose |
|---|---|
| Python | Machine learning, model development, and gesture recognition |
| MediaPipe | Real-time hand detection and landmark tracking |
| CNN | Baseline hand gesture classification |
| GRU | Temporal sequence modeling |
| Unity | Game development and gameplay environment |
| C# | Unity game logic and system integration |

## Model Comparison

MUTED investigates two approaches to hand gesture recognition.

### 1. CNN Baseline

The baseline model uses a Convolutional Neural Network to extract spatial features from hand gesture inputs and classify individual frames.

This approach evaluates gesture recognition without explicitly modeling temporal dependencies between consecutive frames.

### 2. CNN + GRU

The hybrid model combines CNN-based feature extraction with a Gated Recurrent Unit (GRU).

The GRU processes sequential information, allowing the model to learn temporal patterns and relationships between consecutive hand gesture inputs.

### Experimental Comparison

| Aspect | CNN Baseline | CNN + GRU |
|---|---|---|
| Feature Extraction | CNN | CNN |
| Temporal Modeling | No explicit temporal modeling | GRU |
| Input Approach | Individual frames | Frame sequences |
| Primary Focus | Spatial gesture features | Spatial and temporal features |
| Research Role | Baseline model | Temporal modeling approach |

## Dataset and Performance

| Specification | Details |
|---|---|
| Dataset Size | Approximately 5,600 samples |
| Model Architectures | CNN and CNN + GRU |
| Training Environment | Developer's local machine |
| Hand Tracking | MediaPipe |
| Target Frame Rate | 30 FPS |
| Game Engine | Unity |
| Game Scripting | C# |

## System Architecture

The system integrates computer vision, deep learning, and game development to enable real-time gesture-based interaction.

### General Workflow

1. **Hand Capture** – A camera captures the player's hand movements.
2. **Hand Detection** – MediaPipe detects and tracks hand landmarks.
3. **Gesture Recognition** – The custom CNN or CNN+GRU model processes the gesture input.
4. **Prediction Processing** – The recognized gesture is translated into a corresponding game command.
5. **Game Interaction** – Unity receives the recognized input and executes the corresponding in-game action.

## Installation

MUTED is distributed through a standalone installer, making installation simple and straightforward.

### Installation Steps

1. Navigate to this repository's **Releases** section.
2. Download the latest MUTED installer (`MUTED-Setup.exe`).
3. Locate the downloaded installer on your computer.
4. Double-click the installer to launch the setup wizard.
5. Follow the on-screen installation instructions.
6. Once installation is complete, launch MUTED using the desktop shortcut or Start Menu entry, if available.

### System Requirements

- Windows operating system
- Webcam or camera for real-time hand tracking
- Camera access permissions
- Stable lighting conditions for better hand detection

### Important Notes

- A working camera is required for hand gesture-based gameplay.
- Ensure that your camera is accessible before launching the game.
- Position your hand within the camera's visible area for reliable detection.
- For the best experience, use the game in a well-lit environment.

## Development Team

**CSA1**

**Project Lead:** Angelito Flordeliza

**Project Type:** Thesis Research and Development

## Project Significance

MUTED is more than a gesture-controlled game. It is an experimental platform designed to examine an important aspect of real-time gesture recognition: the role of temporal information.

By implementing both a conventional CNN baseline and a CNN+GRU architecture, the project provides a practical environment for investigating whether sequence-based modeling is necessary or beneficial for hand gesture-driven interaction.

The findings can contribute to the development of more responsive and effective gesture recognition systems for interactive applications.

---

**Developed by CSA1**

*Led by Angelito Flordeliza*

*Thesis Project*
