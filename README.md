# TrueSight Pulse ActiveMQ Meter Plugin

This meter plugin collects metrics from the ActiveMQ node using the embedded [Jolokia](https://jolokia.org/) instance that allows measurement collection via a REST API.

### Prerequisites

#### Supported OS

|     OS    | Linux | Windows | SmartOS | OS X |
|:----------|:-----:|:-------:|:-------:|:----:|
| Supported |   v   |    v    |    v    |  v   |

This plugin is compatible with ActiveMQ 5.10.0 or later.

#### TrueSight Pulse Meter Versions V4.5.0-778 or later

- To install new meter go to Settings->Installation or [see instructons|https://help.boundary.com/hc/en-us/sections/200634331-Installation].
- To upgrade the meter to the latest version - [see instructons|https://help.boundary.com/hc/en-us/articles/201573102-Upgrading-the-Boundary-Meter].

### Plugin Setup

None

### Plugin Configuration Fields

|Field Name    |Description                                              |
|:-------------|:--------------------------------------------------------|
|pollInterval  |How often should metrics be gathered from ActiveMQ?      |
|host  |The server from which ActiveMQ stats should be gathered  |
|broker_name |The name of the ActiveMQ broker which should be monitored|
|port  |The port on which ActiveMQ metrics can be retrieved      |
|username  |The administrative user which can gather ActiveMQ metrics|
|password  |The password for the administrative user                 |
|sourceName |The source name to be displayed for each metric |

### Metrics Collected

|Metric Name             |Description                                                                |
|:--------------------------------|:------------------------------------------------------------------------|
|ACTIVEMQ_BROKER_TOTALS_QUEUES    |The total number of ActiveMQ queues active on this node                  |
|ACTIVEMQ_BROKER_TOTALS_TOPICS    |The total number of ActiveMQ topics active on this node                  |
|ACTIVEMQ_BROKER_TOTALS_PRODUCERS |The total number of data producers for ActiveMQ on this node             |
|ACTIVEMQ_BROKER_TOTALS_CONSUMERS |The total number of data consumers for ActiveMQ on this node             |
|ACTIVEMQ_BROKER_TOTALS_MESSAGES  |The total number of messages being processed by ActiveMQ on this node    |
|ACTIVEMQ_BROKER_STATS_ENQUEUE    |The total number of messages written to queues by ActiveMQ on this node  |
|ACTIVEMQ_BROKER_STATS_DEQUEUE    |The total number of messages read from queues by ActiveMQ on this node   |
|ACTIVEMQ_BROKER_STATS_INFLIGHT   |The total number of messages currently in flight in ActiveMQ on this node|
|ACTIVEMQ_MESSAGE_STATS_DISPATCH  |The total number of messages dispatched by ActiveMQ on this node         |
|ACTIVEMQ_MESSAGE_STATS_EXPIRED   |The total number of messages expired by ActiveMQ on this node            |
|ACTIVEMQ_MESSAGE_STATS_QUEUE_SIZE|The total queue size of queues managed by ActiveMQ on this node          |
|ACTIVEMQ_MEM_USED                |The total memory used by ActiveMQ on this node                           |
|ACTIVEMQ_STORE_USED              |The total storage used by ActiveMQ on this node                          |

### Dashboards

- ActiveMQ Summary

### References

None
