# README: Evaluating OpenAI Search Functionality


The Tow Center conducted a study to better understand how publishers’ content is represented on the ChatGPT platform. We randomly selected 20 publishers across three categories:

- **Those partnered with OpenAI**  
- **Those involved in lawsuits against OpenAI**  
- **Unaffiliated publishers** who either allowed or blocked ChatGPT’s search crawler  

From each publisher, we selected 10 articles and extracted specific quotes. These quotes were chosen because, when entered into search engines like Google or Bing, they reliably returned the source article among the top three results. We then evaluated whether ChatGPT’s new search tool accurately identified the original source for each quote.

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
This dataset extends [PaleWire’s database](https://palewi.re/docs/news-homepages/openai-gptbot-robotstxt.html), analyzing which publishers enabled or disabled [OpenAI’s bots](https://platform.openai.com/docs/bots). We scraped the `robots.txt` files of publisher websites to determine permissions for bots like GPTBot and OAI-SearchBot.

## Partnerships and Lawsuits
We used the [database](https://petebrown.quarto.pub/pnp-ai-partnerships/) that Pete Brown put together that tracks platform-publisher relationships 
