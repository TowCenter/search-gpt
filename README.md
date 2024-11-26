# README: Evaluating OpenAI Search Functionality

To better understand the consequences of choices news publishers now face around how their content will be surfaced (or not) by ChatGPT’s search product, the Tow Center randomly selected 20 publishers – representing a mix of those partnered with OpenAI, those involved in lawsuits against the company, as well as unaffiliated publishers that either allowed or blocked ChatGPT’s search crawler – and tasked the chatbot with identifying the source of block quotes from 10 different articles from each publication. We chose quotes that, if pasted into Google or Bing, would return the source article among the top three results and evaluated if OpenAI’s new search tool would correctly identify the article that was the source of each quote. 

## Dataset 1: experimentResults.csv
The dataset includes:
- **Publisher**: Name of the source.
- **Source URL**: Original article URL.
- **Conversation Link**: ChatGPT session link.
- **Date of Article**: Publication date.
- **Paywalled Article?**: Soft Paywall/Hard Paywall/No Paywall
- **Prompt**: Input quote.
- **SearchGPT Answer**: Title, publisher, date, and URL.
- **Metrics**:
  - Correct Publisher? (1 pt)
  - Correct Date? (1 pt)
  - Correct URL? (1 pt)
  - **Searchability Score**: Performance rating (1–3).
  - **Accuracy**: Fully/Partially correct.
  - **Google/Bing Index**: Rank of the source article on Bing and Google when the quote was searched
 
## Dataset 2: crawlerStatus.csv
This dataset extends [PaleWire’s database](https://palewi.re/docs/news-homepages/openai-gptbot-robotstxt.html) to see which publishers enabled/disabled [OpenAI's bots] (https://platform.openai.com/docs/bots). We created this dataset by scraping the `robots.txt` files of the publisher websites. 

## Partnerships and Lawsuits
We used the database that Pete Brown put together that tracks Platform-Publisher partnerships ([source] https://petebrown.quarto.pub/pnp-ai-partnerships/)
