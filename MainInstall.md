# NodeRED_ESPEASY_AutoDiscovery
[Start](README.md)  
[Device Install](Devices.md)  
[Advance Settings](Advance.md)  

# Install Node-Red Flow  
1. Copy [MQTTDiscovery.json](MQTTDiscovery.json) and import in Node-Red
2. Change/Update the MQTT nodes with correct security and other settings
3. Deploy it
4. run inject button Save List to create a starting point.
![NodeRed Flow](PNG/Flow_Node-Red_Install.PNG)

# EasyESP:  
Setup EasyESP:  
**Controller:**  
![EasyEsp Controller](PNG/Controller.PNG)

Controller Subscribe: EE/%sysname%/#

Controller Publish: EE/%sysname%/%tskname%/%valname%

Will Retain: True  

if the device needs to use MQTT import device then you need 2 mqtt controllers configurated the same  
but the first has to not have any username or password and can be disabled.  

## Update Node-Red Flow
1. Renmame the old flow to MQTT Discovery(Old)
2. do Install Node-Red Flow steps
3. press Clear list and Save List to redo all devices
4. Test the Flow 
5. Combine Inject node Settings if it was changed
