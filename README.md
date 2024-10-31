# Coffee Alerter

## Overview
The **Coffee Alerter** is a machine learning project designed to help coffee drinkers monitor their caffeine intake. Using OpenCV, the program utilizes live footage from a webcam to detect when a user drinks from a mug. It tracks the number of gulps taken and alerts the user when the maximum safe caffeine limit is reached.

## Features
- **Real-time video processing**: Captures live footage from your webcam.
- **Gulp detection**: Increases gulp count only when the mug is near the user's mouth.
- **Caffeine tracking**: Calculates total caffeine intake based on average gulp volume.
- **Alert system**: Notifies users when the maximum safe caffeine limit is reached.
- **User-friendly interface**: Displays the number of gulps taken and total caffeine intake on the video feed.

## Requirements
- Python 3.x
- OpenCV
- NumPy
- playsound

## Installation
Install the required packages:
   ```bash
   pip install opencv-python numpy playsound
   ```

3. Ensure you have an alert sound file named `alert.mp3` in the project directory for notifications. The same has been attached also if you are too lazy to search and download one.

## Usage
1. Connect your webcam to the computer.
2. Run the script:
   ```bash
   python coffee_limiter.py
   ```
3. The live feed will open and the quanitites will be shown on the top left corner. The program will display the live video feed, showing the mouth region and detected cup.

4. Press `q` to exit the program.

## Configuration
- The maximum safe coffee intake limit is set to **300 mg** by default.
- The average gulp volume is set to **50 ml**, which can be adjusted in the code.
- Change the `AVG_GULP_VOLUME` and `SAFE_COFFEE_LIMIT` constants in the code as needed.

## Contributing
Contributions are welcome! If you have suggestions or improvements, please fork the repository and create a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- Special thanks to the OpenCV community for providing the tools necessary to create this project.
