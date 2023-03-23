# RPA-UiPath-QueueReport

This Reusable Asset can be used to generate excel report for Queue items from any UiPath Queue for specific duration(Example - Monthly/Weekly/Daily.)
In UIPATH there is limitation at a time from queue maximum 100 queue items can be retrieved. This can be used for more than 100 Queue records also.
 It can be filtered for New,Success,Failed,InProgress,Deleted Queue items.
Input need to provide - Start and End date, Queue Name, need to specify Specific Content – do get input from queue and Excel report file path.
Output – Excel Report
Input:
In_ExcelReportFilePath: Excel FilePath for Queue Report
In_QueueName: UiPath Queue Name

UiPath Queue report :

1. This flow will create Excel report from UIPATH Orchestrator queue items, it can be used to generate reports for more than 100 Queue items .
2.  Assign Start date and End Date of report.
3.  Build Data table with columns which will be used to store data from queue items and write in excel file as Queue Report.
4. Get Total Queue items from UIPATH specific queue - In UIPATH there is limitation at a time from queue maximum 100 queue items can be retrieved.
5.  Flow will go in loop for each 100 queue items, each queue item details will be added to data table.
6. Excel template with required Headers will kept in specific path/location for Queue Report.
7. When all queue item records will be retrieved and added to data table flow will remove old records from excel file and add write new records from Deta table to excel file.

Developed Reusable workflows that makes debugging and troubleshooting less time consuming.
It will save development effort across use cases.
It can help in speeding up the RPA Queue Report for Daily/Weekly/Monthly reports
Can be reutilized in workflows where Bot needs to send Daily/Weekly/Monthly Reports to RPA support Team/Business/End Users.

To use this Code -

Tou need to keep excel report templatewith required headers as per process  in specific path and update that path in input variable in code
update Queue name
update Queue specific values which are required in Report 
Run Code
