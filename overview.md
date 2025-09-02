---

copyright:
  years:  2025
lastupdated: "2025-09-02"

keywords:

subcollection: observability-hub
---

{{site.data.keyword.attribute-definition-list}}


# Overview
{: #overview}

{{site.data.keyword.cloud}} offers Observability services that you can use to monitor, troubleshoot, and understand the activity in your account. You can also use them to keep records for auditing and compliance.
{: shortdesc}

As a user of the {{site.data.keyword.cloud_notm}} you and your customers might need to understand the following for the services that are running:

* The actions that are being taken by services running in your account. For example, if a new user is authorized to use a service.

* Any log entries that are posted while a service is being run. For example, if a service generates a log entry indicating a connection error.

* The health and performance of your service instances. For example, if you are approaching memory limits.

{{site.data.keyword.cloud_notm}} provides observability services that will help you visualize, alert and troubleshoot on your data as well as routing services that you can use to define how to manage and route platform telemetry data in your account.

![IBM Cloud Observability services overview](/images/Observability_services_overview.svg "An overview of the IBM Cloud Observability services, the types of data they process and route and the various destinations for the data."){: caption="Observability services overview" caption-side="bottom"}

## Analysis and storage
{: #analysis-storage}

{{site.data.keyword.cloud_notm}} provides the following services that will help you visualize and alert on your data and help with your observability requirements:

* {{site.data.keyword.logs_full_notm}}
* {{site.data.keyword.mon_full_notm}}

## Collect and route observability data
{: #collect-route}

{{site.data.keyword.cloud_notm}} provides the following platform routing services to configure how data is routed from the source to the appropriate {{site.data.keyword.logs_full_notm}} or {{site.data.keyword.mon_full_notm}} instance. Or, in the case of {{site.data.keyword.atracker_full_notm}} to other supported services such as {{site.data.keyword.cos_full_notm}} or {{site.data.keyword.messagehub}}.

* {{site.data.keyword.logs_routing_full_notm}} - Routes logs.
* {{site.data.keyword.metrics_router_full_notm}} - Routes metrics.
* {{site.data.keyword.atracker_full_notm}} - Routes {{site.data.keyword.cloud_notm}} platform activity tracking events.


## Observability solutions
{: #solutions}

You can also send logs and metrics to {{site.data.keyword.cloud_notm}} Observability solutions from your environments and applications to be visualized and routed.

The following are examples of solution architectures that use the Observability services for service management in IBM Cloud:

- [Three tier application on VMware Cloud Founction as a Service across Multi Zone Region.](/docs/vcfaas-on-mzr?topic=vcfaas-on-mzr-web-app-multizone)

- [IBM Power® Virtual Server resiliency on AIX](/docs/pattern-pvs-aix-resiliency?topic=pattern-pvs-aix-resiliency-power-virtual-server-on-AIX)

- [Cloud foundation for security and observability](/docs/deployable-reference-architectures?topic=deployable-reference-architectures-core-security-services-pattern)
