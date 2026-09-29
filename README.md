# AirMove · Touchless Gesture Control

> Captures hand movements via an ordinary camera and maps palm/finger gestures to cursor movement and clicks, controlling computers, smart TVs, conference displays, and other devices like a mouse—no touching, no remote needed.

[中文](README_CN.md) | English


## Table of Contents
- [Introduction](#introduction)
- [Demo Videos](#demo-videos)
- [Features](#features)
- [Technical Specifications](#technical-specifications)
- [How It Works](#how-it-works)
- [Application Scenarios](#application-scenarios)
- [Environment Requirements](#environment-requirements)
- [Application Directions](#application-directions)
- [License](#license)

## Introduction
AirMove is a vision-based touchless gesture interaction solution. It uses a camera to recognize hand keypoints in real time, tracks palm position and open/closed state, and converts them into screen-cursor movement, clicking, and dragging—achieving "touchless" control of computers, TVs, conference displays, and other devices.

## Demo Videos
The following are real-usage screen recordings; click to play:

**Computer Control (palm movement = cursor movement)**
<video src="./media/demo-pc-control.mp4" controls muted></video>

**Big-screen Control Demo**
<video src="./media/demo-big-screen.mp4" controls muted></video>

**Interactive Game Demo (fishing game)**
<video src="./media/demo-fish-game.mp4" controls muted></video>

**More Control Clips**
<video src="./media/demo-control-clip.mp4" controls muted></video>


## Features
- Real-time hand detection and 21 3D keypoint tracking
- Palm position → cursor movement; fist/open → click/drag
- Supports 1–3 m long-distance big-screen interaction
- Pure vision solution, no hardware to wear
- Low latency, smooth control of desktop and media playback

## Technical Specifications
| Item | Parameter |
|------|-----------|
| Control Precision | 1080 / 720 / 480 / 240 |
| Operation Distance | 0.5 m – 4 m |
| Depth of Field Range | 5× |
| Response Time | < 0.1 s |
| Sampling Frame Rate | 30 fps |
| Control Angle | 72° – 120° |
| Working Mode | Mouse, command (types customizable) |
| Usage Environment | Indoor, outdoor |
| Tracking Precision | Zienon's proprietary anti-shake technology (< 1 pixel) |
| Noise Resistance | Zienon's proprietary noise-resistance technology (three modes) |
| Customized Application | Five-level performance/speed customization configuration |
| Operating System | Windows / Android |

## How It Works
1. Camera captures video frames;
2. Hand detection model locates the palm and outputs 21 3D keypoints;
3. Maps palm-center coordinates to screen coordinates (with smoothing filter);
4. Triggers mouse events (move / left-click / drag) based on finger open/closed state or gesture;
5. Injects events into the system input to control the target device.

## Application Scenarios
- **Living Room**: Touchless control of smart TV and set-top box
- **Meeting Room**: Touchless page-turning and annotation on big screens during presentations
- **Exhibition / Retail**: Contactless interactive big screens
- **Computer**: Replace the mouse for long-distance operation

## Environment Requirements
- Windows / macOS / Linux device with a camera
- Target devices: computer, Android TV, smart TV, etc.

## Application Directions

- **Smart TV / Set-top Box**: Touchless control of TV and set-top box
- **Smart Home**: Gesture wake-up and cross-device linkage
- **Media Interaction**: Touchless interaction for exhibition / big screens
- **Robots**: Touchless commands and control
- **Gesture-recognition Medical Devices**: Contactless operation
- **Gesture Early-education Games**: Children's touchless interactive content

> Zienon Technology holds relevant invention patents (product materials) and provides standardized product capabilities (product parameters).


## License
© Zienon Technology. See LICENSE (supplement the license file if open-sourcing is required).
