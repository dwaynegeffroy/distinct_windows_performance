# distinct_windows_performance
 Windows performance monitoring app for Splunk
 
 Copyright 2021- Dwayne Geffroy
 
# Windows performance monitoring app for Splunk
  
Gain insights into infrastructure using CPU, Memory, Disk and Metrics in Splunk

## Dashboards
- Contains overview dashboards for views across your whole environment, as well as metrics and drill downs for more advanced insights.

![Overview](https://user-images.githubusercontent.com/10578846/127149427-b67420fd-2d3b-4a8f-a1d8-6349566a0839.PNG)
![host_status](https://user-images.githubusercontent.com/10578846/127149651-c3861cce-897f-41c4-8117-eead2bb8f4d5.PNG)

## Reports
- Create and manage thresholds and host information with reports that will fill with information when run

## Alerts
- Comes with alerts for Host Status, Network, CPU, Memory, Paging File and Disk, ranging from simple to advanced alerts.
- Easily modify individual servers for easy management of host or application needs.

# Getting Started

## Prerequisite Apps
Splunk_TA_windows(Standard windows data)

*TA_Performance_Inputs(only if you don't already have the neccessary data activated)

## Steps
1. Download and install distinct_windows_performance to splunk search head
2. Install TA_Performance_Inputs to apply the needed inputs to Splunk forwarders on windows
3. Ensure you setup the macro to the correct index
4. move inputs.conf from TA_Performance_Inputs/default to local, or confirm you have the correct data.
5. activate reports and alerts for full experience, many of the dashboards have sections driven by this.

## Activating and Using Reports
In order to get the most from this app you may need to activate some of the existing reports which will feed the dashboards.

## Create Host_List 
This report creates a csv named host_list.csv, by running this report regularly it will keep this list upto date. This is used in dashboards to speed up looking for host data.

## Update Host_status
This report creates a csv named host_status.csv, by running this report regularly you will keep a list of server responsiveness over time. Keeps upto 10 days of data. Used in dashboards and alerts.

## Threshold Creation Reports
There are a number of threshold lookups that get created for this app, however the thresholds lookups are only neccessary if you intend to modify thresholds on individual servers, you can modify these as needed to ensure any servers can be updated as needed.

