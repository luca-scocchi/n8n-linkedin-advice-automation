# Architecture

The workflow follows a linear, modular pipeline that can be easily extended or customized.

## High-level flow

Trigger
→ Topic Definition  
→ Google / SerpAPI Search  
→ URL Extraction & Deduplication  
→ Article Fetch (HTML)  
→ Content Parsing  
→ AI Contribution Generation  
→ Output (Slack / Database)

## Design principles

- Stateless execution
- Clear separation between discovery, analysis, and generation
- Provider-agnostic AI layer
- Swappable output and storage nodes

## Extensibility

The architecture allows:
- Adding approval steps before publishing
- Replacing search providers
- Supporting multiple AI models
- Integrating additional delivery channels
