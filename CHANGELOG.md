# Changelog
## [1.0.1] - 2025-01-28
### Changed
- Migrated to modern `pyproject.toml` packaging (PEP 621 compliant)
- Restructured project to use `src/` layout for better packaging practices
- Consolidated all dependencies into `pyproject.toml`
- Added UV package manager support with lock file management
- Moved `utils/` directory into `vex` package for proper distribution
- Removed legacy `setup.py` and `requirements.txt` files
- Made `pyaudio` an optional dependency (install with `vex[audio]`)

### Added
- UV installation instructions in README.md
- Support for UV lock file management (`uv.lock`)
- Optional dependencies group for audio features (`[audio]` extra)

### Previous Changes and Fixes (from earlier 1.0.1 release)
- Internal: replaced custom vexEnum with Python’s Enum; no user-facing API changes.
- Removed vexnumber; affected APIs now accept float.
- Moved sleep and wait to a new module vex_util (removed from vex_types).
- Color class updated to accept web color strings.
- Updated move_with_vectors parameter order to the latest specification.
- Minor typos and docstring formatting issues for improved autocomplete tooltip suggestions in VSCode

## [1.0.0] - 2025-04-11
### Features
- **WebSocket Communication**: Establish and manage WebSocket connections for commands, status updates, images, and audio.
- **Robot Control**: Move, turn, and stop the robot with precise control over speed and direction.
- **Sensor Access**: Retrieve data from the robot's inertial sensor, vision system, and touch screen.
- **Screen Interaction**: Draw shapes, display text, and show emojis on the robot's screen.
- **Sound Playback**: Play built-in or custom sounds and musical notes.
- **LED Control**: Set the color of the robot's LEDs.
- **AI Vision**: Detect objects, colors, codes, and AprilTags using the robot's built-in AI features.
- **Camera**: Streaming images from the robot's camera for implementing computer vision applications on the client side.
- **Event Handling**: Register callbacks for screen presses, crashes, and timers.

### Notes
- This is the initial public release.
