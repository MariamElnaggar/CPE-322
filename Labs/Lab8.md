# Data Analysis
I used this code to install the python packages `pip install -U numpy scipy scikit-learn matplotlib pandas keras` I didn;t have any problems installing the `tenserflow` package so I didn't use docker
![CommandLine1](/Images/DataAna1.png)
After that I tested the code using
```
$ python keras_diabetes.py
$ python keras_first_network.py
```
![CommandLine1](/Images/DataAna2.png)
![CommandLine1](/Images/DataAna6.png)
![CommandLine1](/Images/DataAna7.png)
![CommandLine1](/Images/DataAna8.png)
![CommandLine1](/Images/DataAna9.png)

## Google Sheets Graphs
In Lab 7, I used cpu_spreadsheet.py so I have memory available instead of temprature in my data.
The graphs from Google sheets:
![CommandLine1](/Images/DataAna3.png)

I then used this code to copy the files to demo:
```
$ cd ~/demo
$ cp ~/iot/lesson8/plt_final.py .
$ cp ~/iot/lesson8/plt_cv2.py .
```
I then used the following commands to edit the python files to fit my data. 
1. Changing Temprature to Memory Available
2. Changing the titles of the graphs
3. Changing the file the data is read from
4. Changing the x-ticks for figure 1
```
$ nano plt_final.py
$ nano plt_cv2.py
```
![CommandLine1](/Images/DataAna4.png)
![CommandLine1](/Images/DataAna5.png)
