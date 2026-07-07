# AI Integration

Likha AI activities use Control Room AI Settings. This lets users bring their own provider, endpoint, key, model, and request settings.

![Likha Control Room - AI Settings](images/control-room-ai-settings.png)

## AI Activities

- [AI Capabilities.md](Activities/AI%20Capabilities/AI%20Capabilities.md)
- [AI Prompt.md](Activities/AI%20Capabilities/AI%20Prompt.md)
- [AI Extract Documents Fields.md](Activities/AI%20Capabilities/AI%20Extract%20Documents%20Fields.md)
- [AI Vision.md](Activities/AI%20Capabilities/AI%20Vision.md)
- [AI Table Extract.md](Activities/AI%20Capabilities/AI%20Table%20Extract.md)
- [AI Knowledge Search RAG.md](Activities/AI%20Capabilities/AI%20Knowledge%20Search%20RAG.md)

## Smart Rule-Based Operations

Smart operations are not provider-based AI calls. They are local rule, regex, and fuzzy matching helpers.

- [Smart Operations](Activities/Smart%20Operations/README.md)

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

