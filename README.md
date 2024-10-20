
# Football Analysis with Computer Vision

This project focuses on using computer vision techniques to analyse football matches. By utilising **YOLO (You Only Look Once)** for object detection and **OpenCV** for image processing, the project can track and analyse football players' movements and key moments during a match. This analysis can provide insights into player positioning, team strategies, and game patterns.

## Features

- **Player Detection:** Detect football players in video footage using YOLO's real-time object detection capabilities.
- **Movement Tracking:** Track player movement across the pitch using OpenCV for video frame analysis.
- **Zone Heatmap:** Generate heatmaps to visualise which zones players spend the most time in.
- **Key Moment Detection:** Identify key moments such as goals, fouls, and possession changes through visual cues and manual tagging.
- **Performance Metrics:** Extract metrics like distance covered, speed, and player proximity during a match.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/username/football-analysis-cv.git
   cd football-analysis-cv
   ```

2. Set up a virtual environment (optional but recommended):

   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scriptsctivate`
   ```

3. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Download the pretrained YOLO model weights from the [YOLO website](https://pjreddie.com/darknet/yolo/) and place them in the `model/` directory.

2. To analyse a video, run the following command:

   ```bash
   python analyse_video.py --input <path_to_video> --output <output_directory>
   ```

   For example:

   ```bash
   python analyse_video.py --input videos/match.mp4 --output results/
   ```

3. The output will include a summary of key metrics, heatmaps, and annotated video frames saved in the output directory.

## Project Structure

- `analyse_video.py`: Main script to analyse video footage of football matches.
- `models/`: Directory containing the YOLO model weights and configuration files.
- `utils/`: Utility functions for video processing, heatmap generation, and metric calculation.
- `videos/`: Sample football match videos (not included in the repo).
- `results/`: Generated analysis results such as heatmaps and processed videos.

## Requirements

- Python 3.7+
- OpenCV
- YOLO (You Only Look Once) model
- NumPy
- Matplotlib

To install dependencies:

```bash
pip install -r requirements.txt
```

## Future Work

- **Real-time Analysis:** Implement live match analysis from real-time video streams.
- **Tactics Recognition:** Detect and analyse team formations and tactics using more advanced models.
- **Enhanced Key Moment Detection:** Automate the detection of more complex events like offside, penalties, and set-pieces.

## Contributing

Contributions are welcome! If you have suggestions for improvement or would like to report a bug, feel free to open an issue or submit a pull request.

## Sample output
- View a sample output video here: https://drive.google.com/file/d/1n-EUl6D-aBWeVOVGCN7Mlnzqpz4Bxife/view?usp=sharing
