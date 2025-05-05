# ThingSpeak and Google Sheets
## ThingSpeak
I logged into ThingSpeak using my MathWorks account, and created a channel with 2 fields.
![Data](/Images/ThingSpeak4.png)
Then I ran the following commands:
```
$ pip install -U psutil
$ cd ~/demo
$ cp ~/iot/lesson7/thingspeak_cpu_loop.py .
$ cp ~/iot/lesson7/thingspeak_feed.py .
$ cat thingspeak_cpu_loop.py
$ cat thingspeak_feed.py
$ python thingspeak_feed.py
```
![Data](/Images/ThingSpeak3.png)
I then got my Write API key for ThingSpeak and ran the following command and put in my API key when asked
```
$ python thingspeak_feed.py
An API key savefile was not found. Enter Write API Key >>>
Should we save this key for future use? [y/N] >>>
```
I let the code run for a while to get some data points. This was what I got in the terminal: 
![Data](/Images/ThingSpeak1.png)

This was my output on ThingSpeak:
![Graphs](/Images/ThingSpeak2.png)

## Google Sheets
I ran the following command to set up gspread and oauth2client
```
pip install -U gspread oauth2client
```
I followed the following steps after login in to Google Cloud Platform Identity and Access Management:
1. Click "Create" and enter the project name, e.g., rpidata
2. ≡ > APIs & Services > + Enable APIs & Services > Enable both Drive API and Sheets API
3. Credential > Create Credentials > Create service account key > Service account > rpidata > JSON key type > Create > download rpidata-xxxxxxxxxxxx.json

I then set up my spreadsheet.
![CommandLine1](/Images/GoogleSheets1.png)
I ran the following code:
```
$ cd demo
$ cp ~/iot/lesson3/system_info.py .
$ cp ~/iot/lesson7/cpu_spreadsheet.py .
$ mv ~/Downloads/cpudata-*.json ~/demo 
```
Then I edited the cpu_spreadsheet.py file to include the JSON key and ran the cpu_spreadsheet.py file. 
I let the program run for some time, and it populated the spreadsheet.
![CommandLine1](/Images/GoogleSheets2.png)
![CommandLine1](/Images/GoogleSheets3.png)
