# Awesome Azure Security [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of awesome Microsoft Azure Security tools, guides, blogs, and other resources.

## Contribute

Contributions welcome! Read the [contribution guidelines](CONTRIBUTING.md) first.

## Contents

- [Tools](#tools)
  - [Security Assessment Tools](#security-assessment-tools)
  - [Offensive Tools](#offensive-tools)
  - [Infrastructure as Code Scanning Tools](#infrastructure-as-code-scanning-tools)
  - [Other Tools](#other-tools)
- [Threat Detection and Response](#threat-detection-and-response)
  - [Audit Logging](#audit-logging)
  - [Native Alerting](#native-alerting)
- [Blog Posts](#blog-posts)
  - [Offensive blog posts](#offensive-blog-posts)
  - [Defensive blog posts](#defensive-blog-posts)
- [Training](#training)
- [Talks](#talks)
- [Other key resources](#other-key-resources)


# Tools

### Security Assessment Tools

- [Azucar](https://github.com/nccgroup/azucar): Security auditing tool for Azure environments. Windows only. [![stars](https://badgen.net/github/stars/nccgroup/azucar)](https://badgen.net/github/stars/nccgroup/azucar)
- [BloodHound](https://github.com/BloodHoundAD/BloodHound): BloodHound uses graph theory to reveal hidden relationships and attack paths in an Active Directory environment that would otherwise be impossible to quickly identify.  [![stars](https://badgen.net/github/stars/BloodHoundAD/BloodHound)](https://badgen.net/github/stars/BloodHoundAD/BloodHound)
- [ScoutSuite](https://github.com/nccgroup/ScoutSuite): Multi-Cloud Security auditing tool. [![stars](https://badgen.net/github/stars/nccgroup/ScoutSuite)](https://badgen.net/github/stars/nccgroup/ScoutSuite)
- [Steampipe](https://github.com/turbot/steampipe): Instantly query your cloud, code, logs & more with SQL. Build on thousands of open-source benchmarks & dashboards for security & insights. [![stars](https://badgen.net/github/stars/turbot/steampipe)](https://badgen.net/github/stars/turbot/steampipe)
- [StormSpotter](https://github.com/Azure/Stormspotter): Azure Red Team tool for graphing Azure and Azure Active Directory objects. [![stars](https://badgen.net/github/stars/Azure/Stormspotter)](https://badgen.net/github/stars/Azure/Stormspotter)


### Offensive Tools

- [MicroBurst](https://github.com/NetSPI/MicroBurst): a PowerShell Toolkit for Attacking Azure. [![stars](https://badgen.net/github/stars/NetSPI/MicroBurst)](https://badgen.net/github/stars/NetSPI/MicroBurst)
- [PowerZure](https://github.com/hausec/PowerZure): a PowerShell project created to perform reconnaissance and exploitation of Azure, AzureAD, and the associated resources. [![stars](https://badgen.net/github/stars/hausec/PowerZure)](https://badgen.net/github/stars/hausec/PowerZure)
- [ROADrecon](https://github.com/dirkjanm/ROADtools): a tool for exploring information in Azure AD from both a Red Team and Blue Team perspective. [![stars](https://badgen.net/github/stars/dirkjanm/ROADtools)](https://badgen.net/github/stars/dirkjanm/ROADtools)


### Infrastructure as Code Scanning Tools

- [Checkov](https://github.com/bridgecrewio/checkov): Terraform, Cloudformation and Kubernetes static analysis written in python. [![stars](https://badgen.net/github/stars/bridgecrewio/checkov)](https://badgen.net/github/stars/bridgecrewio/checkov)
- [Terraform Compliance for Azure](https://github.com/turbot/steampipe-mod-terraform-azure-compliance): Steampipe module to check compliance of Terraform configurations to Azure security best practices. [![stars](https://badgen.net/github/stars/turbot/steampipe-mod-terraform-azure-compliance)](https://badgen.net/github/stars/turbot/steampipe-mod-terraform-azure-compliance)
- [tfsec](https://github.com/tfsec/tfsec): Provides static analysis of your terraform templates to spot potential security issues. [![stars](https://badgen.net/github/stars/tfsec/tfsec)](https://badgen.net/github/stars/tfsec/tfsec)


### Other Tools

- [DumpsterDiver](https://github.com/securing/DumpsterDiver): Tool to search secrets in various filetypes like keys (e.g. AWS Access Key Azure Share Key or SSH keys) or passwords. [![stars](https://badgen.net/github/stars/securing/DumpsterDiver)](https://badgen.net/github/stars/securing/DumpsterDiver)

# Threat Detection and Response

### Audit Logging
- [Azure security logging and auditing](https://docs.microsoft.com/en-us/azure/security/fundamentals/log-audit): Azure provides a wide array of configurable security auditing and logging options to help you identify gaps in your security policies and mechanisms.

### Native Alerting
- [Azure Security Center - Alerts Reference Guide](https://docs.microsoft.com/en-us/azure/security-center/alerts-reference): This article lists the security alerts you might get from Azure Security Center and any Azure Defender plans you've enabled.

# Blog Posts

### Offensive blog posts

- [Attacking Azure Cloud Shell](https://blog.netspi.com/attacking-azure-cloud-shell/) by [Karl Fosaaen](https://twitter.com/kfosaaen): Leveraging Azure Cloud Shell storage files with subscription contributor permissions to perform cross-account command execution and privilege escalation.
- [Nuking all Azure Resource Groups under all Azure Subscriptions](https://kmcquade.com/2020/11/nuking-all-azure-resource-groups-under-all-azure-subscriptions/) by [Kinnaird McQuade(@kmcquade3)](https://twitter.com/kmcquade3): How to abuse Azure Resource hierarchy and tenant-wide god-mode Service Principals to nuke an entire Azure environment.
- [Privilege Escalation and Lateral Movement on Azure](https://medium.com/xm-cyber/privilege-escalation-and-lateral-movement-on-azure-part-1-47e128cfdc06) by [Hila Cohen (@hilaco10)](https://twitter.com/hilaco10): some techniques for how a red team can gain a foothold in an Azure environment, escalate their privileges, and move laterally inside Azure infrastructure by using the Azure RBAC module and common Azure misconfigurations.
- [Privilege Escalation in Azure AD](https://emptydc.com/2020/12/10/privilege-escalation-in-azure-ad/) by [Jan Geisbauer (@janvonkirchheim)](https://twitter.com/janvonkirchheim): a breakdown of how Azure security principals (aka Enterprise applications) vs application objects (aka application registrations) and their associated permissions can be abused to impersonate an application.
- [Privilege Escalation and Lateral Movement on Azure](https://medium.com/xm-cyber/privilege-escalation-and-lateral-movement-on-azure-part-1-47e128cfdc06): some techniques for how a red team can gain a foothold in an Azure environment, escalate their privileges, and move laterally inside Azure infrastructure by using the Azure RBAC module and common Azure misconfigurations.
- [Abusing Azure AD SSO with the Primary Refresh Token](https://dirkjanm.io/abusing-azure-ad-sso-with-the-primary-refresh-token/): Most corporate devices have Primary Refresh Tokens - long term tokens stored on your laptop or other AD connected resources - for Single Sign On (SSO) against on-prem and Azure AD connected resources. See Dirk-jan Mollema's blog goes over abusing these tokens, which you can access if you have code execution on a target or on your laptop that is Azure AD joined.

### Defensive blog posts

- [Detect Azure network configuration mistakes with visualization using Flow Logs and Traffic Analytics](https://autosysops.com/blog/use-traffic-analytics-to-spot-common-azure-network-mistakes) by [Leo Visser (@AutoSysOps)](https://twitter.com/autosysops): Use Traffic Analytics and Flow Logs in Azure to spot network configuration mistakes by visualizing your flows. This tool gives you multiple different visual graphs to spot mistakes and malicious behavior.
- [Use Azure API Management and Keyvault to authorize based on API body values](https://autosysops.com/blog/control-api-arguments-per-team-with-azure-api-management) by [Leo Visser (@AutoSysOps)](https://twitter.com/autosysops): There are times where you want to limit certain values in a POST request to specific teams/people. This could be build into the API itself, but you can also use serverless techniques in Azure to manage this for you and keep your overall API less complex. This will reduce the attack vector of your overall API.

## Training

- [Awesome Azure Learning](https://github.com/ddneves/awesome-azure-learning): numerous references for Azure learning, especially for the Azure Certs, Azure Architecture, and any other learning materials e.g. Security topics. [![stars](https://badgen.net/github/stars/ddneves/awesome-azure-learning)](https://badgen.net/github/stars/ddneves/awesome-azure-learning)
- [Azure AZ 500 Study Guide](https://github.com/AzureMentor/Azure-AZ-500-Study-Guide): Study Guide for the Microsoft Azure Security Technologies Exam. [![stars](https://badgen.net/github/stars/AzureMentor/Azure-AZ-500-Study-Guide)](https://badgen.net/github/stars/AzureMentor/Azure-AZ-500-Study-Guide)
- [Azure AZ 500 Labs by Microsoft](https://github.com/MicrosoftLearning/AZ500-AzureSecurityTechnologies): Study Guide for the Microsoft Azure Security Technologies Exam. [![stars](https://badgen.net/github/stars/MicrosoftLearning/AZ500-AzureSecurityTechnologies)](https://badgen.net/github/stars/MicrosoftLearning/AZ500-AzureSecurityTechnologies)
- [Breaking and Pwning Apps and Servers on AWS and Azure](https://github.com/appsecco/breaking-and-pwning-apps-and-servers-aws-azure-training): Course content, lab setup instructions and documentation of our very popular Breaking and Pwning Apps and Servers on AWS and Azure hands on training. [![stars](https://badgen.net/github/stars/appsecco/breaking-and-pwning-apps-and-servers-aws-azure-training)](https://badgen.net/github/stars/appsecco/breaking-and-pwning-apps-and-servers-aws-azure-training)

# Talks

# Other key resources

