# Structured Output Performance

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://e7zy.short.gy/G1LklQ)

A comparison of structured output performance among popular open and closed source large language models.

## Local Setup

### Install dependencies

`poetry install --no-root`

### API Keys

Copy `.env.example` to `.env` and add your API keys.

## Potential Improvements

- Measure tokens per second
- Add Anthropic models
- Update Groq to use `with_structured_output`
- Break out GPT 4 versions
- Ensure instance of class isn't empty
- Add ability to mix in different Pydantic objects and prompts
- Parallelize
- Create a version that doesn't use LangChain

### Caveats

This analysis is performed with one, fairly simple prompt template, run with just 10 samples per model. More complicated prompts/tasks will negatively impact consistency. And tinkering with different prompt strategies will improve consistency. It's also important to note, quality/accuracy of output is not considered here, only consistency and latency.
