# yt-embed-generator

A lightweight, client-side tool that converts a YouTube link into an embeddable iframe player and generates the corresponding embed code.

The project is intentionally simple and dependency-free, focusing on correctness, usability, and a clean user interface.

## Features
- Accepts multiple YouTube URL formats:
  - https://www.youtube.com/watch?v=VIDEO_ID
  - https://youtu.be/VIDEO_ID
  - https://www.youtube.com/shorts/VIDEO_ID
  - https://www.youtube.com/embed/VIDEO_ID
  - Raw 11-character video IDs
- Instantly renders an embedded player preview
- Generates copy-ready iframe embed code
- Optional redirect to the original YouTube watch page
- Responsive layout for desktop and mobile
- No external libraries or frameworks

## How it works
The tool extracts the YouTube video ID from user input and constructs a valid `/embed/VIDEO_ID` iframe.  
All processing is done locally in the browser; no data is sent to any server.

## Running locally
Recommended method:

```bash
python3 -m http.server 8000

