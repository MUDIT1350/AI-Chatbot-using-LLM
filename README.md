# AI-Chatbot-Based on-LLM
🌐 A Python-based web research AI Chatbot based on LLM that automatically searches the internet to answer user questions. Built with web scraping and search capabilities.

✨ Features
🔍 Google Search Integration: Uses Google Search to find relevant web pages

🦆 DuckDuckGo Fallback: Automatic fallback to DuckDuckGo if Google fails

📚 Wikipedia Integration: Direct API access to Wikipedia for factual queries

🤖 Smart Content Extraction: Extracts and summarizes relevant information from web pages

📊 Relevance Scoring: Ranks information based on query relevance

🔗 Source Tracking: Keeps track of all sources with titles and URLs

💬 Interactive CLI: Easy-to-use command-line interface

📋 Prerequisites
Python 3.6+

Internet connection

Google Search API access (through googlesearch-python library)

🚀 Installation
Clone the repository:

bash
git clone https://github.com/yourusername/internet-research-bot.git
cd internet-research-bot
The bot will automatically install required packages on first run, or you can manually install them:

bash
pip install requests beautifulsoup4 google
🎯 Usage
Run the bot:

bash
python research_bot.py
Example Queries:
text
What is artificial intelligence?
How does photosynthesis work?
Who is Albert Einstein?
Explain quantum computing
Tell me about the Mars Rover
Commands:
Type quit, exit, bye, or q to exit

Press Ctrl+C to exit immediately

🏗️ Architecture
Main Components:
InternetResearchBot Class: Core bot functionality

Search Methods:

search_google(): Primary search using Google

search_duckduckgo(): Fallback search using DuckDuckGo

Content Processing:

fetch_page_content(): Downloads and cleans webpage content

extract_key_info(): Extracts relevant sentences based on query

summarize_content(): Creates concise summaries

Knowledge Sources:

Wikipedia API for factual queries

Multiple web sources for comprehensive answers

Workflow:
User inputs a question

Bot identifies query type (factual → Wikipedia, general → web search)

Searches multiple sources

Extracts and scores relevant information

Generates concise answer with sources

⚙️ Configuration
The bot uses sensible defaults, but you can modify:

num_results in search_google(): Number of search results to process

time.sleep(1): Delay between requests (be polite to servers)

text[:3000] in fetch_page_content(): Maximum content length per page

🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

Areas for Improvement:
Add more search engines

Improve summarization algorithms

Add caching mechanisms

Implement async requests for faster searches

Add GUI interface

Add export functionality (JSON, PDF, etc.)

⚠️ Limitations
Rate limiting by search engines

Website anti-scraping measures

Quality depends on source reliability

May not handle very complex queries perfectly

Requires active internet connection

📝 License
This project is open source and available under the MIT License.

👨‍💻 Author
Mudit Shanker Saxena

🙏 Acknowledgments
googlesearch-python library for search functionality

Wikipedia for their excellent API

All the open-source libraries that make this possible

⭐ Support
If you find this project useful, please give it a star! ⭐
