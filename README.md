YouTube Video Analytics & Sentiment Analysis

A Python-based tool that performs comprehensive analysis of YouTube videos by extracting metadata, comments, and transcripts, then applies advanced sentiment analysis to understand audience engagement and emotional responses.

Features
Video Metadata Extraction: Get video title, channel info, view counts, likes, and thumbnails

Comment Analysis: Extract and process user comments with like counts and timestamps

Transcript Retrieval: Access video transcripts when available

Sentiment Analysis: Classify comments into emotional categories (positive, negative, neutral, joyful, angry, sarcastic, etc.)

Batch Processing: Efficiently analyze large volumes of comments using Groq's LLM API

Data Visualization: Generate insights and distributions of audience sentiment

Detailed Reporting: Create comprehensive video analysis reports

Installation
Clone the repository:

bash
git clone <your-repo-url>
cd youtube-sentiment-analysis
Install required dependencies:

bash
pip install google-api-python-client pandas youtube-transcript-api langchain-groq
Set up your API keys:

YouTube Data API v3 key

Groq API key

Usage
python
# Configure your API keys
DEVELOPER_KEY = 'your_youtube_api_key'
GROQ_API_KEY = 'your_groq_api_key'

# Analyze a YouTube video
video_id = "7ntHBqTGHVc"
# The tool will extract comments, analyze sentiment, and generate insights
Project Structure
youtube_data_extraction.py - Handles YouTube API interactions

sentiment_analysis.py - Processes comments using Groq LLM

comment_processor.py - Manages batch processing of comments

visualization.py - Creates charts and insights

config.py - API configuration and settings

API Requirements
YouTube Data API v3: For video metadata and comments

Groq API: For LLM-powered sentiment analysis

youtube-transcript-api: For closed caption extraction

Output
Processed comments with sentiment labels

Sentiment distribution charts

Video engagement metrics

Audience reaction insights

Emotional response analysis

Use Cases
Content creators analyzing audience reception

Marketing agencies measuring campaign effectiveness

Researchers studying social media engagement

Brand monitoring and reputation management
