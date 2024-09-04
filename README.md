# AI New Generation
This project automates the process of generating an AI news by leveraging a team of AI agents that fetch, analyze, and compile the latest news stories into a well-formatted markdown document.
## Overview
This project uses the `crewai` framework to manage multiple AI agents that work together to produce a daily AI newsletter. The agents are powered by a large language model (LLM) and are responsible for various tasks such as fetching news, analyzing articles, and compiling the final news.
## Features
- **Automated News Fetching**: The `NewsFetcher` agent gathers the latest AI news stories.
- **Intelligent Analysis**: The `NewsAnalyzer` agent breaks down the news into digestible summaries with critical insights.
- **Newsletter Compilation**: The `NewsletterCompiler` agent assembles the analyzed content into a well-formatted markdown newsletter.
## Installation
To set up this project, follow these steps:
1. Clone the repository:
    ```bash
    git clone https://github.com/Adityajeet/multi_agent.git
    cd multi_agent
    ```
2. Create a virtual environment and activate it:
    ```bash
    python -m venv myenv
    # On Windows use `myenv\Scripts\activate`
    ```
3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```
4. Set up environment variables:
   - Create a `.env` file in the root directory.
   - Add your Google API key to the `.env` file:
     ```
     SERPER_API_KEY = your_serper_api_key
     GOOGLE_API_KEY=your_google_api_key
     ```
## Usage
To generate the AI news, run the following command:

```bash
python main.py
