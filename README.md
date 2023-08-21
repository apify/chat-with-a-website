# Chat with a website

Chat with a website using Apify and ChatGPT.

## Setup

Before getting started, be sure to sign up for an [Apify](https://console.apify.com/sign-up) and [OpenAI](https://openai.com/) account and create API keys.

To set up and run this project, follow these steps:

1. Install the required packages with `pip`:
   ```
   pip install -r requirements.txt
   ```
2. Rename the `.env.example` file to `.env` and replace the variables. Here's an explanation of the variables in the .env file:

`OPENAI_API_KEY`: Your OpenAI API key. You can obtain it from your OpenAI account dashboard.  
`APIFY_API_TOKEN`: Your Apify API token. You can obtain it from [Apify settings](https://console.apify.com/account/integrations).  
`WEBSITE_URL`: The full URL of the website you'd like to chat with.  

3. Run the `scrape.py` script to scrape the website's data using Apify's [Website content crawler](https://apify.com/apify/website-content-crawler).
4. Run the Streamlit chat app, which should default to `http://localhost:8501` and allow you to chat with the website:
   ```
   streamlit run chat.py
   ```
