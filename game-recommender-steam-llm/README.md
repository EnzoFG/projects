# Steam Game Recommender (LLM + Steam API)

A game recommendation system that analyzes a Steam user's library, playtime and reviews, and uses an LLM (OpenAI GPT-4o mini) together with classic NLP techniques to suggest personalized games.

Academic project for the Natural Language Processing course at UFABC (2024-Q2).

## What it does

- Pulls a user's public Steam data (owned games, playtime) through the Steam Web API.
- Collects game reviews from the Steam `appreviews` endpoint.
- Applies NLP techniques to the reviews: summarization, keyword extraction, translation, emotion detection and sentiment analysis.
- Plots playtime with matplotlib.
- Prompts an LLM with the user's profile to generate personalized game recommendations.

## Stack

Python · OpenAI API (GPT-4o mini) · python-steam-api · steamreviews · requests · matplotlib · Google Colab

## How to run

1. Open `game_recommender_steam_llm.ipynb` in [Google Colab](https://colab.research.google.com/) (or Jupyter).
2. Install the dependencies: `pip install -r requirements.txt`.
3. Get your keys:
   - OpenAI API key: https://platform.openai.com/api-keys
   - Steam Web API key: https://steamcommunity.com/dev/apikey
4. Run the notebook. Keys are requested at runtime with `getpass`, so they are never stored in the file.
5. Enter a public Steam profile ID when prompted.

## Privacy note

Outputs were cleared and no keys or personal data are committed. The Steam profile you query must be public.

## Author

Enzo Fujita Garcia
