# Voiceflow Perplexity Reasoning Extension

Integrate Perplexity AI's reasoning capabilities into your Voiceflow widget for step-by-step reasoning and professional responses.

## Features

- Step-by-step reasoning visualization
- Professional and succinct responses
- Support for Perplexity's Sonar reasoning models
- Real-time streaming of reasoning and answers

## Setup

1. Get a Perplexity API key from [Perplexity API](https://docs.perplexity.ai/)
2. Import the example agent file: `Perplexity_Reasoning_(Extension)-2025-02-19_13-57.vf`
3. Set your API key in the project {ppxApiKey} variable

## Usage

You can use this payload in your custom action, fell free to modify the system prompt:

```json
{
  "apiKey": "{ppxApiKey}",
  "model": "{model}",
  "messages": [
    {
      "role": "system",
      "content": "You are an expert. Keep your reasoning succinct and spoken professionally"
    },
    {
      "role": "user",
      "content": "{last_utterance}"
    }
  ]
}
```

### Available Models

- `sonar-reasoning`: Standard reasoning model
- `sonar-reasoning-pro`: Enhanced reasoning capabilities
- `sonar-pro`: Pro model without reasoning capabilities
- `sonar`: Standard model without reasoning capabilities

## Resources

- [Perplexity API Documentation](https://docs.perplexity.ai/)
- [Voiceflow Documentation](https://www.voiceflow.com/docs)
