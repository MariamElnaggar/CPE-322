# YANG
I ran the following command to install YANG and PlantUML
```
$ pip install pyang plantuml
```
After that I used the following commands to copy the code needed to my demo folder and set my current directory to demo
```
$ cp ~/iot/lesson9/intrusiondetection.yang ~/demo
$ cd demo
```
Then, I used the following code to convert the YANG file to a YIN file, then convert the YANG file to UML format, and then used the UML file to create a diagram using PlantUML
```
$ pyang -f yin -o intrusiondetection.yin intrusiondetection.yang
$ pyang -f uml -o intrusiondetection.uml intrusiondetection.yang --uml-no=stereotypes,annotation,typedef
$ python -m plantuml intrusiondetection.uml
```
Resualting in this diagram:
![CommandLine1](/Images/YANG1.png)

## Terminal Output
![CommandLine1](/Images/YANG2.png)
