---
layout: default
---

<nav class="doc-home-link"><a href="https://burnimjerome.github.io/LIKHA-_-BETA/">&larr; Go back Home</a></nav>

# Extract Details From...

**Activity group:** AI Screen Control

## Purpose

Extracts requested details from a visible application screen and returns them as structured data. The activity is useful when an agent or workflow needs specific values from a form, record, dialog, dashboard, or legacy application instead of the complete screen text.

The activity activates and inspects the selected target window before extracting the requested details. It can use the visible screenshot, OCR text, and available Windows UI information as context.

## Properties

- `Target Window`: `Automatic` selects the topmost visible non-Likha window. Enter part of a window title to target a specific application.
- `Details to Extract`: Describes the fields or facts to return. Use clear field names and expected meanings.
- `Output`: Object variable containing the extracted field names and values.
- `Status Code`: Number variable that receives the AI request HTTP status code.
- `Timeout`: Maximum AI request time in seconds.
- `Retry`, `Retry Count`, `Retry Interval`, and `On Error`: Standard execution and failure behavior.

## Example

```txt
Target Window: Finance Application
Details to Extract: Customer Name, Invoice Number, Invoice Date, Total Amount, and Status
Output: ScreenDetails
Status Code: ExtractDetailsStatusCode
Timeout: 90
```

Example output:

```json
{
  "Customer Name": "Acme Trading",
  "Invoice Number": "INV-1048",
  "Invoice Date": "2026-07-14",
  "Total Amount": "12500.00",
  "Status": "Pending"
}
```

## Recommended Use

1. Keep the target application visible and unlocked.
2. Specify only the details required by the next workflow or agent step.
3. Store the result in an Object variable.
4. Validate required fields before using them in a submission, payment, or irreversible action.
5. Use [AI Verify Screen](AI%20Verify%20Screen.html) when the flow must confirm the application state after an action.

Use [AI Read Screen](AI%20Read%20Screen.html) when you need all visible text and layout. Use **Extract Details From...** when you need a smaller, named set of values.

