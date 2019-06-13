# Python Binding

 Frida Support the python binding

**Sample**

``` python
import frida, sys
 
ss = """
Java.perform(function () {
 //logic goes here
"""
device = frida.get_usb_device()
pid = device.spawn(["sg.vantagepoint.root"])
session = device.attach(pid)
script = session.create_script(ss)
script.load()
device.resume(pid)
raw_input()
```

1)Download the File

2)Reverse the apk

3)Find the logic

4)Create the python script to bypass the logic


5) save it in the **.py** extension

6) Run the **python** File

```
python l3.py
```
