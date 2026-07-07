# Excel Automation

Excel activities work with an ExcelInstance created by Launch Excel.

## Excel Activities

- [Launch Excel.md](Activities/Excel%20Automation/Launch%20Excel.md)
- [Read Excel.md](Activities/Excel%20Automation/Read%20Excel.md)
- [Read Cell Excel.md](Activities/Excel%20Automation/Read%20Cell%20Excel.md)
- [Write Excel.md](Activities/Excel%20Automation/Write%20Excel.md)
- [Write Cell Excel.md](Activities/Excel%20Automation/Write%20Cell%20Excel.md)
- [Get Workbook Sheet Excel.md](Activities/Excel%20Automation/Get%20Workbook%20Sheet%20Excel.md)
- [Get Last Row Column Excel.md](Activities/Excel%20Automation/Get%20Last%20Row%20Column%20Excel.md)
- [Execute Macro Excel.md](Activities/Excel%20Automation/Execute%20Macro%20Excel.md)
- [Close Excel.md](Activities/Excel%20Automation/Close%20Excel.md)

## Read Range Behavior

Read Range saves rows into a DataTable variable.

Blank cells are normalized to empty text.

Fully blank rows and trailing blank columns are ignored.

## Recommended Pattern

1. Launch Excel.
2. Read Range into a DataTable.
3. Use For Each to process rows.
4. Write results back to Excel or another system.
5. Close Excel with the desired save option.

