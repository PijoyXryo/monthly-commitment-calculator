# Monthly Commitment Calculator

A desktop app for tracking monthly financial commitments (loans, bills, subscriptions) against your income. Built with Python and [customtkinter](https://github.com/TomSchimansky/CustomTkinter).

<!-- Add a screenshot: drag an image into this file on GitHub, or save it as docs/screenshot.png -->

## Features
- Enter your monthly income and add commitments with a name, amount and due date (from a calendar picker)
- **Load meter** that shows what percentage of your income is already committed
- Browse commitments by month and year
- Dark / light mode toggle
- Export the current view to **CSV** or a formatted **PDF** report (ReportLab)
- Data saved locally to `data.json`, so there's no account or internet needed

## Run it
```bash
pip install customtkinter reportlab
python "Monthly Commitment Calculator.py"
```

## Project structure
```
Monthly Commitment Calculator.py   entry point
app.py                             main window, UI and export logic
calendar_popup.py                  custom date-picker widget
data.py                            JSON load/save + RM currency formatting
theme.py                           colour palette and dark/light themes
```

## What I learned
- Structuring a GUI app into separate modules for UI, data, theme and widgets instead of one big script
- Building a custom widget (the calendar popup) from scratch
- Generating PDF reports programmatically with ReportLab
