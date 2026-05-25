# Specs: CSV Export Button

## Requirements
- The page MUST display an "Export CSV" button on the reports page
- The button MUST download a .csv file when clicked
- The file MUST contain all data visible in the report
- The filename SHOULD include the current date (e.g. report-2026-05-25.csv)
- The button MUST be disabled when there is no data to export

## Scenarios

### Scenario 1: User exports data successfully
- Given: the user is on the reports page with data loaded
- When: they click the "Export CSV" button
- Then: a .csv file is downloaded to their device

### Scenario 2: No data available
- Given: the reports page has no data
- When: the user sees the "Export CSV" button
- Then: the button is greyed out and cannot be clicked
