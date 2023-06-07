# Bookmarks2Notion

This is a Python script that uses the BeautifulSoup and requests libraries to scrape web pages, then uses the OpenAI API to process the scraped information and finally creates a new page in Notion using the notion_client library.

## Screenshots

![image](https://github.com/CarlosUlisesOchoa/Bookmarks-to-Notion/assets/26280134/28354a47-1e06-4c1e-8a06-8e4f8d9ff2f1)

![image](https://github.com/CarlosUlisesOchoa/Bookmarks-to-Notion/assets/26280134/335ecaf3-4c75-413c-8c74-fa07dcbf2720)

![image](https://github.com/CarlosUlisesOchoa/Bookmarks-to-Notion/assets/26280134/9046cab8-bfb4-4e66-8c2a-51d193a97f55)

## Environment Variables

The script uses environment variables to configure some settings. These variables must be declared in a `.env` file, which must be located in the same directory as the script. Here are the environment variables used:

- `BOOKMARKS_FILE`: The path to a file containing the URLs to be processed.
- `OPENAI_API_KEY`: The API key to access OpenAI's API.
- `NOTION_API_KEY`: The API key to access Notion's API.
- `NOTION_DB_ID`: The ID of the Notion database where the pages will be created.
- `USER_AGENT`: The User-Agent header value to be used when making HTTP requests.
- `LANGUAGE`: The language to be used when processing the scraped information with OpenAI's language model.

## How to Run

1. Rename `.env.template` to `.env` and set the proper values

2. Add your URL's inside the file you specified. (default is bookmarks.txt)

3. Install the required Python packages using pip.

```
pip install -r requirements.txt
```

4. Run the script:

```
python main.py
```

The script will read the URLs from the bookmarks file, scrape each web page, process the scraped information, and create a new page in Notion.

