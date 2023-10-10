# WAF20 Baseline (draft)

It is intended to be part of the chapter "Establish a baseline" from the WAF 20 draft article:
https://review.learn.microsoft.com/en-us/azure/well-architected/security/establish-baseline?branch=collab-waf-2-0-1

## Common IT environment used as a baseline

WAF Security is based on Zero Trust pillars to help companies identify and group resources of the same type together and additionally understand how Azure security solutions may be applied as recommendations for different types of resources to have your environment secure.

Network, Infrastructure, Endpoint, Application, Data, and Identity are the pillars considered in this baseline and it will be also used to demonstrate how a common IT environment may be securely protected.

The below logical diagram will be used as a reference throughout the Recommendations provided in this WAF Security documentation, so you may easily identify how to associate WAF security recommendations with specific resources, and then how to apply them in your own environment.

![image](https://github.com/rudneir2/WAF20-baseline-draft-/assets/97529152/5fa47020-17fb-4c24-9367-9611e0cb97de)

**The logical diagram presents four main layers.**

### Infrastructure baseline

This is considered a common IT environment, with an on-premises layer with basic resources utilized in most companies and an Azure public cloud layer with common services used by most companies as well.

### Azure Security services

This layer presents some of the most common Azure security services grouped according to the WAF pillars and the types of resources they protect. You may find a complete set of Azure security services under Azure Security benchmarks:
https://learn.microsoft.com/en-us/security/benchmark/azure/overview 

### Azure Monitoring

This layer presents the Monitoring services available on Azure that go beyond simple monitoring services, including SIEM and SOAR solutions and Microsoft Defender for Cloud.

**1) Log Analytics**
Responsible for storing all the logs from Azure resources and Azure security services. It is also used to set up the log archive and do log ingestion transformation before logs are stored.

**2) Azure Monitor**
It offers a set of features to monitor Azure resources metrics, like CPU usage among others, alerts management, Application monitoring, etc.

**3) Microsoft Sentinel**
This is the SIEM and SOAR solution based on the cloud. No infrastructure like servers and a bunch of disks are necessary to run your SIEM.

**4) Microsoft Defender for Cloud**
Also known as MDC, this Security solution offers a series of Recommendations to your Azure resources to have a better security environment plus some workload protections and an Alert system based on machine learning and Microsoft Security Graphs API, that is capable of correlating Microsoft security knowledge database with your Azure resources that may be compromised.

All services below will be detailed in the Monitoring Recommendations chapter.

### Threats
This layer brings a recommendation and reminder that threats may be mapped according to your Company's concerns regarding Threats, regardless of the methodology or matrix-like Mitre Attack Matrix or Cyber Kill chain.

** In the following chapters you will have this baseline used as a reference to explain workload examples that may benefit from the Recommendations provided by this WAF Security documentation.
