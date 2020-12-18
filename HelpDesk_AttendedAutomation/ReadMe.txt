Helpdesk Agent Assisted Bot:

Agent Assistant Robot trigger the bot with Hotkey keyboard trigger(ALT +S) by the Agent.
The bot reads the Request.xlsx from the 'Requests' folder,The excel file has the content of the helpdesk ticket.
New workflow called"ReadExcelRequest.XAML" is invoked to read the content of the Excel ticket request file and store those in seperate variables.
The output arguments from this workflow are inputed as the input arguments to the next invoked workflow called "ZohoAutomation.XAML". This workflow will create a helpdesk ticket in Zoho desk application.
Once the ticket is created , the request.xlsx file will be moved to the 'Processed' folder
The Agent can place another 'request.xlsx' file in the Request folder and use 'ALT +S' to create the ticket
The Agent has to use the 'STOP' option in the UiPath Studio to stop the automation.

Note:
Zoho website will be continously updated if the automation failed then you need to update the selectors used in this project before you try it again. It can be easily performed by just using the "Indicate on Screen" Option"

