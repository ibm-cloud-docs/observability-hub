---

copyright:
  years:  2024
lastupdated: "2024-12-16"

keywords:

subcollection: observability-hub
---

{{site.data.keyword.attribute-definition-list}}

# Working with the Observability deployable architecture
{: #deployable-architecture}

IBM Cloud Observability services are available as a deployable architecture called "Cloud Automation for Observability". The "Cloud Automation for Observability" deployable architecture can be used as a building block with other services. Observability services deployment can be automated using {{site.data.keyword.cloud_notm}} Projects. {{site.data.keyword.cloud_notm}} Projects manages related resources and deployments across accounts, embracing an Infrastructure as Code (IaC) approach to deployments. 
{: shortdesc}

## What is Cloud Automation for Observability?
{: #cloud-automation-observability}

Cloud Automation for Observability is a preconfigured set of infrastructure as code (IaC) assets that is deployed and configured based on recommended best practices. This architecture lets your team efficiently deploy and manage your Observability services environment. This architecture simplifies the deployment and configuration of the Observability service that provide you the visibility into applications, services and the activity in your account.

## Proviosning Observability instances
{: #cloud-automation-observability-instances}

This deployable architecture provisions the following Observability instances:

* {{site.data.keyword.logs_full_notm}} 
* {{site.data.keyword.mon_full_notm}}

## Configuring Observability routing services
{: #cloud-automation-observability-routing-services}

* {{site.data.keyword.atracker_full_notm}} is used to configure routing of activity tracking events in the account.
* {{site.data.keyword.logs_routing_full_notm}} is used to configure routing of platform logs in the account


![IBM Cloud Observability deployable architecture](/images/deployable-architecture-observability-instances.svg "An overview of the IBM Cloud Observability deployable architecture."){: caption="Observability Instances deployable architecure" caption-side="bottom"}


This deployable architecture lets you simplify your organization's observability configuration and automate its maintenance. It also supports provisioning of a resource group, root keys in an existing key management service (KMS), an {{site.data.keyword.cos_full_notm}} instance and KMS encrypted {{site.data.keyword.cos_full_notm}} buckets. With this deployable architecture, you can:

Easily deploy: Enables the quick deployment of an observability environment after entering the required inputs.

Secure data with KMS encryption: The data related to logs, monitoring and events is encrypted using a pre-configured KMS key, safeguarding data against unauthorized access and ensuring compliance with security standards.

Configure routing of activity tracking events: Supports routing of IBM Cloud platform activity tracking events to an {{site.data.keyword.cos_full_notm}} bucket and to {{site.data.keyword.logs_full_notm}}.

Configure {{site.data.keyword.logs_routing_full_notm}}: Routes the platform logs to {{site.data.keyword.logs_full_notm}}.

Integrate with {{site.data.keyword.en_full_notm}}: {{site.data.keyword.logs_full_notm}} can be integrated with {{site.data.keyword.en_full_notm}} to collect notification events.

Configure {{site.data.keyword.logs_full_notm}} policies
 
## Deploying Cloud Automation for Observability using IBM Cloud Projects
{: #deploy-resources}

1. From the {{site.data.keyword.cloud_notm}} catalog, search for *Cloud Automation for Observability*.
2. Add *Cloud Automation for Observability* to an existing project or create a project.
3. Depending on your use case, you can refer to the following guidance for information about configuring your architecture or building more comprehensive solutions:
    - [Configure](/docs/secure-enterprise?topic=secure-enterprise-config-project) and [deploy](/docs/secure-enterprise?topic=secure-enterprise-deploy-project) from your project.
    - You can [stack deployable architectures](/docs/secure-enterprise?topic=secure-enterprise-config-stack) together in a project to create a robust end-to-end solution architecture. You don't need to code Terraform to connect the member deployable architectures within the stack. As you configure input values in a member deployable architecture, you can reference inputs or outputs from another member to link the deployable architectures together. After you deploy the deployable architectures in your stack, you can add the stack to a private catalog to easily share it with others in your organization.
