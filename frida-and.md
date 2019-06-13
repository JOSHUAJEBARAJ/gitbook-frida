# Installing Frida-Server on android

Download the frida server


[Download-link](https://github.com/frida/frida/releases/download/12.6.6/frida-server-12.6.6-android-x86.xz)

1) Get into the root mode
```
adb root
``` 
2) Push the Frida-server inside the device
```
adb push frida-server /data/local/tmp/ 
```
3) change the permission

```
adb shell "chmod 755 /data/local/tmp/frida-server"

```

4) Start the Frida server
```
adb shell "/data/local/tmp/frida-server &"
 ```

 ## Verification

Run the follow  command to check whether the frida-server was sucessfully started

 ```
 frida-ps -U
 ```
