# YouTube Video to PDF Notes Converter

This Python script allows you to convert a YouTube video into a PDF file containing screenshots of the video at intervals where the content changes significantly. It uses Structural Similarity Index (SSIM) to compare consecutive frames and saves a frame as a screenshot if it is significantly different from the previous frame.

## Installation

Before running the script, ensure you have the necessary libraries installed:

```bash
pip install pytube3 moviepy fpdf pillow scikit-image

# Usage

Replace the url variable in the script with the URL of the YouTube video you want to convert to PDF notes.
Run the script:

The script will download the YouTube video, extract frames, compare them, and save distinct frames as screenshots.
The screenshots are then compiled into a PDF file, which is saved in the output directory as notes.pdf.

# Warning
Please note that this script is not perfect. It may include additional screens such as subscribe pages, like/share requests, or any other non-content frames as distinct slides in the output PDF. Manual cleanup of the generated PDF may be necessary to remove these additional slides.

# License
This project is open-source and available under the MIT License.
