# Sarah OS product documentation

## Product introduction

### 1.1 About SarahOS

SarahOS is a lightweight distributed hardware management system, providing operation and maintenance, application batch management and block chain project mining pool function of the hardware node intelligent, currently the system integrated Filecoin mining procedures.

SarahOS currently supports node that access to the mainstream Linux distribution (including: Ubuntu, CentOS, RedHat, Debian) , and if installing SarahOS SDK on the node, you can manage and schedule their own account under the node through SarahOS monitoring。

### 1.2 Version requirements

SarahOS suggested using the Linux distribution Ubuntu 16.04.

## Function list
`
<table>
    <tr>
    	<td>Module</td>
    	<td>Name</td>
    	<td>Introduction</td>
    </tr>
    <tr>
        <td rowspan="4">
            Node basic management
        </td>
	<td>SDK download</td>
    	<td>Provide SDK download, install to the node, then access to the SarahOS.</td>
    </tr>
    <tr>
    	<td>Node statistics</td>
    	<td>Overview of all node information of account.</td>
    </tr>
    <tr>
    	<td>Node management</td>
    	<td>Detail information of all nodes under the account, including dynamic data and process monitoring.</td>
    </tr>
    <tr>
    	<td>Alarm management</td>
    	<td>Node alarm setup and alert notification.</td>
    </tr>
    <tr>
        <td rowspan="2">
            Task distribution
        </td>
    	<td>Task pane</td>
    	<td>Write a Script using built-in programming language to assign tasks to nodes.</td>
    </tr>
    <tr>
    	<td>Application center</td>
    	<td>Add applications to the desktop and install existing applications to batch notes.</td>
    </tr>
    <tr>
        <td rowspan="3">
            Secondary application
        </td>
    	<td>IPFS</td>
    	<td>IPFS installing program.</td>
    </tr>
    <tr>
    	<td>IPFS</td>
    	<td>IPFS Storage application.</td>
    </tr>
    <tr>
    	<td>Filecoin</td>
    	<td>Filecoin installing program.</td>
    </tr>
</table>


## The name of the function

### 3.1 SDK download

Function description: download the SDK to the node and install the SDK on the node device.

Function points:
```text
(1) download SDK;
(2) Instructions for installation and uninstallation.
```

### 3.2 Node statistics

Function description: according to the monitoring statistics data of each node, check the current operation situation of the mine pool.

Function points:
```text
(1) view hardware resources. Statistics data includes: total number of nodes, total Vcpu, average Vcpu, total memory, total disk space, update time.
(2) node basic monitoring. Statistics data include: average system load, memory usage, disk usage, download bandwidth, upload bandwidth.
(3) node distribution diagram: it shows the distribution of currently connected nodes on the map. 
```

### 3.3 Node management

Function description: operate and manage the nodes connecting the mine pool.

Function points:
```text
(1) view node information. The display information is as follows: node UID, node name, version, status, update period, network address, creation time, startup time, update time.
(2) check monitoring information: the following display information is that: system load, system load, memory occupancy rate, disk occupancy rate, download bandwidth, upload bandwidth, update time, dynamic chart of monitoring load.
(3) check hardware information
	A. Basic information: CPU, memory, storage space, number of network CARDS and network address
	B, BIOS information: supplier, version, release time, run space, ROM space
	C. Hardware system information: manufacturer, product name, version, serial number, UUID
	D. mainboard information: manufacturer, product name, version, serial number
	E. CPU details: CORE_ID, model number, dominant frequency, cache
(4) node management and operation
	A. Check system information. Status, system, node name, kernel version, distribution, architecture
	B. View the list of processes. User, process ID, CPU utilization, memory utilization, virtual memory, physical memory, terminal, state, startup time, running time, process instruction
	C. Restart node. Call terminal interface input command.
````

### 3.4 Alarm management

Function description: monitor the nodes and find abnormal nodes in time

Function points:
```text
(1) view history alerts. The display information is as follows: node UID, node name, alarm type, alarm value, release time, processing status, and tag processing.
(2) alarm setting
	A. Warning setting item: alarm item, system load, memory utilization, disk utilization, upload bandwidth byte/second, download bandwidth byte/second, automatic alarm setting
	B. notification method: SMS, email, WeChat 
	C. Receiver management: name, mobile phone number, email, OpenID of WeChat, add time and update time
```

### 3.5 task panel
Function description: write scripts through the built-in programming language to assign tasks to nodes

Function points:
```text
(1) task information creation and setting. The following settings are : ID, task name, creation time, task description
(2) code input and operation;
(3) check the task status. The following display items are : number of distribution nodes, number of completion nodes, status
```

### 3.6 application center
Function description: add applications to desktop, install existing applications to batch nodes

Function details:
```text
(1) add application: select the application to add to the desktop
(2) opening application: select application and open
```
### 3.7 application distribution and operation: go-ipfs, go-filecoin
Function : installing IPFS and Filecoin program to each node and operating the program on the node.

Function details:
```text
(1) preview of the installed node: view the node status of the installed program.
(2) task list: check the task execution of the issued program.
(3) configuration task: configure different tasks to issue different procedures and nodes. (configuration parameters are as follows: name of the executable program, whether it start, whether process is monitored，whether or not to push the process dynamic data, the application root directory, log directory, data directory, whether  delete the installation files or not when uninstallating, unloading whether delete logs, unloaded whether to delete the data, application initialization command, start command, the PATH environment variable)
```

### 3.8 application -IPFS storage
Function overview: upload files through the IPFS network storage.

Function points:
```text
(1) upload files: upload to IPFS network through the local files
(2) view files: view and download files in IPFS network
```


