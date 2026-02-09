# Nodes Breakdown

## Trigger
Starts the workflow manually or on a scheduled basis.

## Set Topic for Google Search
Defines the expertise topic used to discover LinkedIn Advice articles.

## Google / SerpAPI HTTP Request
Performs a Google search using:
site:linkedin.com/advice <topic>

## Extract Article Links (Code Node)
Parses search results, extracts LinkedIn Advice URLs, and removes duplicates.

## Split Out Links
Processes each article URL individually.

## Fetch Article HTML
Retrieves the full HTML content of each LinkedIn Advice article.

## HTML Extract
Extracts:
- Article title
- Topics
- Existing user contributions

## AI Contribution Writer
Generates original advice using OpenAI or Google Gemini while avoiding repetition.

## Output Nodes
Sends generated contributions to Slack and/or stores them in a database.
