# 1. Content Pack Introduction

Log Insight is the VMware log management system. After the Huawei Log Insight content pack is installed,you can monitor and manage the sysLog logs reported by Huawei rack, blade, and eSight servers, collect log statistics, analyze logs,view event change trends, and pre-customize alarm sending.You can quickly locate server problems and analyze potential server problems.

**Content Pack Name:** 
- Huawei - eSight  v1.0.vlcp
- Huawei - HMM  v1.0.vlcp
- Huawei - iBMC  v1.0.vlcp

**Supported Version:**
- Log Insight 4.0.0 
- Log Insight 4.6.0

**Mapping Software:** 
- eSight: eSight V300R008C00SPC201
- MM910: (U54) 6.86D or later
- iBMC: 2.94 (U25) or later

**Supported Device:**
-   Huawei management server:   eSight
-   Huawei blade server:        E9000
-   Huawei rack server:         RH2288H V2, RH1288 V3, RH2288 V3, RH2288H V3, RH5885 V3, RH8100 V3, 1288H V5, 2288H V5, and 2488 V5
-   Huawei high-density server: XH321 V3, XH620 V3, XH622 V3, and XH628 V3

# 2. Content Pack Functions
## iBMC content pack:
- **Dashboards:** 
The Overview, Security, System, and Operation pages are included. The view functions are as follows:
	- Change trends of different events
	- Statistics on and analysis of events of each server
	- Statistics on login failures, system error events, and operation error events
	- Statistics on proportion views of some events
	- Statistics on and analysis of operation events of each client

- **sysLog log parsing:** parsing of fields and meanings of sysLog events
- **Alarms:** Multiple Login Failure Alert and alarms triggered by major faults on boards

## HMM content pack:
- **Dashboards:** 
The Overview, System, and Operation pages are included. The view functions are as follows:
	- Change trends of different events
	- Statistics on and analysis of events of each server
	- Statistics on login failures, system error events, and operation error events
	- Statistics on proportion views of some events
	- Statistics on and analysis of operation events of each client	

- **sysLog log parsing:** parsing of fields and meanings of sysLog events
- **Alarms:** Multiple Login Failure Alert and alarms triggered by major faults on boards

## eSight content pack:
- **Dashboards:** 
The Overview, Security, System, and Operation pages are included. The view functions are as follows:
	- Change trends of different events
	- Statistics on and analysis of events of each eSight
	- Statistics on login failures, system error events, and operation error events
	- Statistics on proportion views of some events
	- Statistics on and analysis of operation events of each client

- **sysLog log parsing:** parsing of fields and meanings of sysLog events
- **Alarms:** Multiple Login Failure Alert, Multiple SNMP Polling Failure, and Multiple Health Status Polling Failure Alert

# 3. Server Configuration
## iBMC Configuration
1.	Log in to the BMC WebUI as an administrator and choose **Alarm&SEL > Alarm Settings**.

2.	Set the following parameters in the **Syslog Notification Settings** area:
	-	**Syslog Notifications:** Set this parameter to ON.
	-	**Transmission Protocol:** Set this parameter to TCP or UDP.
	-	**Current Status:** Set this parameter to Enable.
	-	**Server Address:** Set this parameter to the IP address of the Log Insight server.
	-	**Syslog Port:** Set this parameter to 514.
	-	Set other parameters as required.

## HMM Configuration
1.	Log in to the BMC WebUI as an administrator and choose **System Management > Remote Syslog**.</b>

2.	Set the following parameters in the **Operation Logs** area:
	- **Syslog Status:** Set this parameter to ON.
	-	**Server Address:** Set this parameter to the IP address of the Log Insight server.
	-	**Transmission Protocol:** Set this parameter to TCP or UDP.
	-	Set other parameters as required.

3.	Set the following parameters in the **System Logs** area:
	-	**Syslog Status**: Set this parameter to ON.
	-	**Server Address**: Set this parameter to the IP address of the Log Insight server.
	-	**Transmission Protocol**: Set this parameter to TCP or UDP.
	-	Set other parameters as required.

## eSight Configuration
1.	Log in to the eSight WebUI as an administrator and Click **?** in the upper right corner to open the eSight help document, choose **System Parameter Settings > Setting eSight Log Forwarding > Enabling Log Forwarding**, and enable the log forwarding function by referring to this section.

2.	Log in to the eSight WebUI as an administrator again and choose **System > System Interconnection > Transfer Settings > Log Transfer Settings**.

3.	Click **+ Create** to access the log forwarding setting page, and set the following parameters:
	-	**Active server IP address:** Set this parameter to the IP address of the Log Insight server.
	-	**Active server port:** Set this parameter to 514.
	-	**Protocol type:** Set this parameter to TCP or UDP.
	-	**Enabled:** Set this parameter to Yes.
	-	Set other parameters as required.
