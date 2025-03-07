---
uid: PIAdapterForAzureEventHubsOverview
---

# PI Adapter for Azure Event Hubs overview

PI Adapter for Azure Event Hubs is a data-collection component that transfers time-series data from Event Hubs to OMF endpoints in AVEVA Data Hub or PI Servers. Event Hubs is a data streaming platform and event ingestion service provided by Microsoft as part of the Azure Cloud platform. The adapter can connect to any Event Hub hosted in Azure that uses the Advanced Message Queueing Protocol (AMQP).

![PI Adapter for Azure Event Hubs architecture](/images/pi-adapter-for-azure-event-hubs-architecture-diagram.png)

## Adapter installation

You can install the adapter with a download kit that you can obtain from the AVEVA Customer Portal. You can install the adapter on devices running either Windows or Linux operating systems.

## Adapter configuration

Using the REST API, you can configure all functions of the adapter. The configurations are stored in JSON files. For data ingress, you must define an adapter component in the system components configuration for each device to which the adapter will connect. You configure each adapter component with the connection information for the device and the data to collect. For data egress, you must specify destinations for the data, including security for the outgoing connection. Additional configurations are available to egress health and diagnostics data, add buffering configuration to protect against data loss, and record logging information for troubleshooting purposes.

Once you have configured the adapter and it is sending data, you can use administration functions to manage the adapter or individual ingress components of the adapter. Health and diagnostics functions monitor the status of connected devices, adapter system functions, the number of active data streams, the rate of data ingress, the rate of errors, and the rate of data egress.

## EdgeCmd utility

OSIsoft also provides the EdgeCmd utility, a proprietary command line tool to configure and administer an adapter on both Linux and Windows operating systems. EdgeCmd utility is installed separately from the adapter.
