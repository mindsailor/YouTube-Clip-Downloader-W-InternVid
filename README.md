[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mindsailor/YouTube-Clip-Downloader-W-InternVid/blob/main/YouTubeClipDownloader.ipynb)


YouTube-Clip-Downloader-W-InternVid
YouTube Clip Downloader with InternVid Dataset Support
This Python script allows you to download video clips from YouTube using the "yt-dlp" library and the "InternVid-10M-FLT" dataset, a subset of the larger "InternVid" dataset. The script extracts frame-level information and saves the data in a structured JSON format for further analysis or use in other applications.

Dataset Information https://huggingface.co/datasets/OpenGVLab/InternVid/
The caption file for the InternVid dataset can be found at Hugging Face Datasets - OpenGVLab/InternVid.








Key Features
Download Video Clips: The script uses "yt-dlp" to download video clips from YouTube using their video IDs and timestamps provided in the JSONL file.

JSONL Input: The input data is read from a JSONL file ("caption.jsonl") that contains information about the YouTube video clips, including video IDs, timestamps, captions, and other metadata.

Multithreading: The script utilizes the ThreadPoolExecutor to download multiple video clips concurrently, improving the download efficiency by utilizing multiple threads.

Frame Count: The script calculates the number of frames in each downloaded video clip using the OpenCV library, which is used to analyze and process the videos.

Filename Formatting: The script formats the output filename for each downloaded video clip by concatenating the YouTube video ID and a truncated version of the caption.

JSON Output: The script generates a JSON output file containing metadata for each downloaded video clip, including video path, number of frames, and frame-level information with frame index and full caption.











License and Citation: The script includes citation information for the "InternVid" dataset, acknowledging the work's source and providing necessary references and license details.

License and Citation
This Python script uses the InternVid dataset from the OpenGVLab/InternVid repository. If you find this work useful for your research, please consider citing the following papers:

"InternVid: A Large-scale Video-Text Dataset for Multimodal Understanding and Generation," Wang, Yi et al. (2023), arXiv preprint arXiv:2307.06942. GitHub repository

"InternVideo: General Video Foundation Models via Generative and Discriminative Learning," Wang, Yi et al. (2022), arXiv preprint arXiv:2212.03191.

The dataset is released under the CC-BY-NC-SA-4.0 license.

Please note that this script is provided as-is and may be subject to updates or changes based on the dataset's development and library dependencies.
