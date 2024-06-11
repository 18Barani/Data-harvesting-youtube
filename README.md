YouTube Data Harvesting README
Overview
This repository contains scripts and tools for harvesting data from YouTube. The scripts leverage the YouTube Data API to collect various types of data including video metadata, comments, and statistics.

Requirements

Python 3.x

Google API client library (google-api-python-client)

YouTube Data API key

Setup

Obtain API Key:


Visit the Google Developers Console.

Create a new project or select an existing one.

Enable the YouTube Data API for your project.

Create an API key and restrict it to the YouTube Data API.

Setup

Obtain API Key:

Visit the Google Developers Console.

Create a new project or select an existing one.

Enable the YouTube Data API for your project.

Create an API key and restrict it to the YouTube Data API.

Install Dependencies:


bash

Copy code

pip install google-api-python-client

Configuration:

Copy the API key obtained in step 1.

Paste the API key into the config.py file.

Authentication:

Ensure your API key has appropriate permissions to access YouTube data.
Usage

harvest_videos.py: Harvests metadata of videos from specified YouTube channels or search queries.

bash
Copy code
python harvest_videos.py --channels CHANNEL_ID1,CHANNEL_ID2,... --search_query "SEARCH_QUERY"
harvest_comments.py: Harvests comments from specified YouTube videos.

bash
Copy code
python harvest_comments.py --video VIDEO_ID

Output

Video Metadata:

videos.json: JSON file containing metadata of harvested videos.
Comments:
comments_VIDEO_ID.json: JSON file containing comments of the specified video.
License
This project is licensed under the MIT License - see the LICENSE file for details.


Acknowledgments
Google Developers for the YouTube Data API.

Disclaimer

This project is for educational and research purposes only. Use responsibly and respect the terms of service of YouTube and Google APIs.
