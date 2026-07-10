---
layout: default
---

# AI Integration

Likha AI activities use Control Room AI Settings. This lets users bring their own provider, endpoint, key, model, and request settings.

Likha supports a Bring Your Own Key model for AI features. This means each user or company connects their own AI provider account instead of sharing a central Likha-owned AI subscription.

![Likha Control Room - AI Settings](images/control-room-ai-settings.png)

## What This Is For

AI Settings are used by AI-powered activities inside Likha, including:

- AI Prompt
- AI Vision
- AI Table Extract
- AI Extract Document Fields
- AI Knowledge Search
- Likha Copilot, when enabled

Once configured, these activities can reuse the same provider endpoint, API key, model, temperature, and token settings.

## Why Bring Your Own Key

Bring Your Own Key gives customers control over:

- AI provider choice
- API usage cost
- model selection
- data handling policies
- provider billing
- organization-level access controls

Likha does not need to resell AI credits for this mode. The customer pays their AI provider directly.

## Supported Provider Type

The current AI Settings screen supports OpenAI-compatible chat completion endpoints.

Example endpoint:

```text
https://api.openai.com/v1/chat/completions

## AI Activities

- [AI Capabilities.md](Activities/AI%20Capabilities/AI%20Capabilities.html)
- [AI Prompt.md](Activities/AI%20Capabilities/AI%20Prompt.html)
- [AI Extract Documents Fields.md](Activities/AI%20Capabilities/AI%20Extract%20Documents%20Fields.html)
- [AI Vision.md](Activities/AI%20Capabilities/AI%20Vision.html)
- [AI Table Extract.md](Activities/AI%20Capabilities/AI%20Table%20Extract.html)
- [AI Knowledge Search RAG.md](Activities/AI%20Capabilities/AI%20Knowledge%20Search%20RAG.html)

## Smart Rule-Based Operations

Smart operations are not provider-based AI calls. They are local rule, regex, and fuzzy matching helpers.

- [Smart Operations](Activities/Smart%20Operations/README.html)

## Configuration

Open:

```text
Control Room > AI Settings
```

Configure:

- Provider
- Endpoint URL
- API key
- Model
- Temperature
- Max tokens

## Typical Use Cases

- Summarize extracted browser or document text.
- Convert free-form text into structured JSON.
- Classify emails or queue items.
- Extract fields from OCR or document output.
- Analyze screenshots, receipts, charts, barcodes, and QR codes.
- Extract table rows from PDFs or images.
- Ask questions from a policy, SOP, folder, or link.

## Notes

Do not hard-code API keys inside workflow steps. Use Control Room AI Settings or secured environment configuration.

