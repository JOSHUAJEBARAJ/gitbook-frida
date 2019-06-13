# Frida Basics

Frida comes with the bunch of tools

## Frida-ps

To check the running process
```
frida-ps -U 
```
To check the running apps
```
frida-ps -Ua

```
To check the running app process
```
frida-ps -Uai
```
## Frida-ls

This tool help to list the devices
```
frida-ls-devices
```
##Hooking to process


```
frida -U [process-name]

frida -U -f [process-name]

frida -U -f [process-name] --no-pause

```
