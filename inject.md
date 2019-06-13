# Injecting Our code using Javascript

## Sample javascript payload
``` javascript

Java.perform(function() {

        var   main = Java.use("sg.vantagepoint.root.MainActivity");

       main.isDeviceRooted.implementation = function() {
            console.log("In function A");
             return false;
         }  
   

});

```

1) Download the apk

[]

2)Try to Find the secret


3) Reverse the apk

4) Try to find the logic


```

frida -U -f [process-name] --no-pause -l [filename]
```
