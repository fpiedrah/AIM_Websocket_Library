# VEX AIM Websocket Python Client

 VEX AIM Websocket Python Client is a Python library designed to interact with the VEX AIM robot over WebSocket connections. It provides a high-level API to control the robot's movements, sensors, screen, sound, and other features from an external device.

## Features

- **WebSocket Communication**: Establish and manage WebSocket connections for commands, status updates, images, and audio.
- **Robot Control**: Move, turn, and stop the robot with precise control over speed and direction.
- **Sensor Access**: Retrieve data from the robot's inertial sensor, vision system, and touch screen.
- **Screen Interaction**: Draw shapes, display text, and show emojis on the robot's screen.
- **Sound Playback**: Play built-in or custom sounds and musical notes.
- **LED Control**: Set the color of the robot's LEDs.
- **AI Vision**: Detect objects, colors, codes, and AprilTags using the robot's built-in AI features.
- **Camera**: Streaming images from the robot's camera for implementing computer vision applications on the client side.
- **Event Handling**: Register callbacks for screen presses, crashes, and timers.

## Installation

### Using UV (Recommended)

[UV](https://github.com/astral-sh/uv) is a fast Python package installer and resolver.

```bash
# Install UV if you haven't already
curl -LsSf https://astral.sh/uv/install.sh | sh

# Install the VEX AIM WebSocket library
uv pip install vex

# Install with audio support (optional)
uv pip install vex[audio]

# Or install from source in development mode
git clone https://github.com/VEX-Robotics/AIM_Websocket_Library.git
cd AIM_Websocket_Library
uv pip install -e .

# Install from source with audio support
uv pip install -e ".[audio]"
```

### Using pip

```bash
pip install vex

# Install with audio support (optional)
pip install vex[audio]

# Or from source
git clone https://github.com/VEX-Robotics/AIM_Websocket_Library.git
cd AIM_Websocket_Library
pip install -e .

# Install from source with audio support
pip install -e ".[audio]"
```

### Optional Dependencies

- **audio**: Adds `pyaudio` for audio streaming features. Install with `vex[audio]` if you need audio capabilities.
  - **Note**: PyAudio can be challenging to install on some systems. If you encounter issues, see the [PyAudio installation guide](https://people.csail.mit.edu/hubert/pyaudio/).
```

## Documentation

For instructions on setting up the library, connecting the robot over Wi-Fi, and exploring the full API, refer to the [AIM WebSocket API pages](https://api.vex.com/aim/home/websocket/index.html).

## License

The library and example code in this project are licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
The VEX AIM firmware and related intellectual property are copyrighted by VEX Robotics. For more information, refer to the [Copyright notice](https://www.vexrobotics.com/copyright-notice) provided by VEX Robotics.

## Support

For any issues or questions, please open an issue on the [GitHub repository](https://github.com/VEX-Robotics/AIM_Websocket_Library/issues).

