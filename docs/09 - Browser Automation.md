# Browser Automation

Browser automation uses BrowserInstance variables and Playwright-backed selectors.

![Likha Process Designer](images/process-designer.png)

## Browser Activities

- [Browser Start.md](Activities/Browser%20Automation/Browser%20Start.md)
- [Browser Attach.md](Activities/Browser%20Automation/Browser%20Attach.md)
- [Browser Go To.md](Activities/Browser%20Automation/Browser%20Go%20To.md)
- [Browser Click.md](Activities/Browser%20Automation/Browser%20Click.md)
- [Browser Fill.md](Activities/Browser%20Automation/Browser%20Fill.md)
- [Browser Press button on web page.md](Activities/Browser%20Automation/Browser%20Press%20button%20on%20web%20page.md)
- [Browser Set checkbox.md](Activities/Browser%20Automation/Browser%20Set%20checkbox.md)
- [Browser Select radio button.md](Activities/Browser%20Automation/Browser%20Select%20radio%20button.md)
- [Browser Set Drop down list.md](Activities/Browser%20Automation/Browser%20Set%20Drop%20down%20list.md)
- [Browser Wait Element.md](Activities/Browser%20Automation/Browser%20Wait%20Element.md)
- [Browser Screenshot.md](Activities/Browser%20Automation/Browser%20Screenshot.md)
- [Browser Extract Text.md](Activities/Browser%20Automation/Browser%20Extract%20Text.md)
- [Browser Extract Table.md](Activities/Browser%20Automation/Browser%20Extract%20Table.md)
- [Browser Click Image.md](Activities/Browser%20Automation/Browser%20Click%20Image.md)
- [Browser Wait Image.md](Activities/Browser%20Automation/Browser%20Wait%20Image.md)
- [Browser Extract Text OCR.md](Activities/Browser%20Automation/Browser%20Extract%20Text%20OCR.md)
- [Browser Run Javascript Function.md](Activities/Browser%20Automation/Browser%20Run%20Javascript%20Function.md)
- [Browser Close.md](Activities/Browser%20Automation/Browser%20Close.md)

## Selector Picker

The browser picker captures properties such as:

- Tag
- ID
- Name and other attributes
- Text
- Classes
- Role
- Form
- Child index
- Ancestor path

Users can choose which properties compose the final selector. Prefer stable attributes such as `name`, `data-testid`, `aria-label`, and `placeholder` when IDs are dynamic.

## Recommended Pattern

1. Add Browser Start or Browser Attach.
2. Use the same BrowserInstance in later browser activities.
3. Pick and highlight selectors before running.
4. Use image/OCR fallback only when DOM selectors are not reliable.

