# Travel Expense Automation

## Overview
This project was created as a final assignment for a self-selected complementary studies course focused on Robotic Process Automation (RPA). The aim was to design and implement an end-to-end business process automation using UiPath and realistic enterprise use cases.

The automation simulates the processing of employee travel expense reports, covering the full workflow from receiving invoices via email to data enrichment in Excel, expense calculations, currency rate lookup through browser automation, report generation, PDF export, email delivery, and archiving of processed items.
The input data was modified instead of using the original course-provided datasets as-is

Although the project originated as a course assignment, the version presented in this portfolio has been refactored and modernized while maintaining the original scope. The project architecture has been restructured, deprecated activities have been replaced with up-to-date UiPath components, and hard-coded values have been minimized by introducing configuration files, DataTables, and LINQ-based data handling.

🎥 **Demo video**: https://youtu.be/FkdWQsn5BK0

## Tech stack
- UiPath Studio (Modern)
- Excel automation
- Browser automation (Google Search)
- DataTables & LINQ
- Gmail integration

## How to run
1. Clone the repository
2. Copy `Data/config.template.xlsx` → `config.xlsx`
3. Fill in your own email address and folder paths
5. Open the project in UiPath Studio
6. Create SMPT/IMAP connections via UiPath's Orchestrator. Otherwise robot won't execute whole process as there is Gmail integration added for demo purposes.
7. Run `Main.xaml`
