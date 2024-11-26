# README: Evaluating OpenAI Search Functionality

This project evaluates OpenAI’s search functionality in ChatGPT by testing its ability to identify the correct sources of quoted content from various publishers. Results were compared to traditional search engines like Google and Bing.

### Objectives
- Assess ChatGPT’s accuracy in identifying original sources for selected quotes.
- Compare its performance with traditional search engines.
- Analyze interactions with publishers across categories: OpenAI partners, litigants, and unaffiliated.

---

## Dataset 1:  
The dataset includes:
- **Publisher**: Name of the source.
- **Source URL**: Original article URL.
- **Conversation Link**: ChatGPT session link.
- **Date of Article**: Publication date.
- **Paywalled Article?**: Yes/No.
- **Prompt**: Input quote.
- **SearchGPT Answer**: Title, publisher, date, and URL.
- **Metrics**:
  - Correct Publisher? (1 pt)
  - Correct Date? (1 pt)
  - Correct URL? (1 pt)
  - **Searchability Score**: Performance rating (1–3).
  - **Accuracy**: Fully/Partially correct.
  - **Google/Bing Index**: Rank of the source article on Bing and Google when the quote was searched
 
