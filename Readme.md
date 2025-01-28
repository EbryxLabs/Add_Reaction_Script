A reaction adding script has been finalised. We will be using this script to add reactions to elastalert messages from now.

Script Working:
This Script adds reaction to alert messages that are posted in the elastalert channel. It basically checks for the messages that are posted in the channel is a duration of last 3 minutes and then adds reaction to them, then it waits for three 3 and then checks for the new messages and add reaction to messages at which there is no reaction added.
It is not only adding reaction to the messages but It will extract the client IP, Alert title, Time at which message was posted, Count of alert, AbuseIPDB reputation and country of the IP Address present in the message and post it into the Excel sheet. Whenever there are multiples same type alerts from the same IP address it increases the count of the that IP Address and updates the time to new time of the message.

Pros:
No Need to add reaction manually to each alert from now onward.
No Need to copy IP Address from each alert.
Get exact count of alerts in your shift by added reactions.
Reduce labour work and saves time for analysis and other tasks.
None of the IP Address is skipped.
IP count, Reputation and Country are at one place

When to Use it:
We have to start the automation when the shift starts, keep it running whole the shift and end it exactly when shift ends. Moreover you can execute it either on Careem laptop or Ebryx laptop.

How to Run it:
Download the attached file and extract it.
Open it folder in VS code.
Install the dependencies using the command pip install -r .\requirements.txt .
Run the Script using python automation.py.
Script will ask for Careem Username which is m.zeeshan@ext.careem.com in my case, you need to give user name and it will keep on adding reactions to messages with emoji associated with you name.
Install Excel Viewer extension in VS code and open the data.xlsx using this extension in VS Code. Because using Microsoft Excel will hault the script when new data is added.
Reopen the same data.xlsx file to see the updated data from sheet.