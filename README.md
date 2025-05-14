# Zabbix - Atlassian Status Page Template
![Zabbix Compatible](https://img.shields.io/badge/Zabbix-Template-blue?logo=zabbix&style=flat-square)

This is a Zabbix template for monitoring components listed on an Atlassian-powered Status Page


## Features

* **Low-Level Discovery (LLD)** of status page components
* **Component Status Monitoring** (eg. Operational, Degraded, Partial Outage, Major Outage)
* **Mapped Status** using value maps
* **Triggers** (Disabled By Default) for component states
	* Degraded Performance
	* Partial Outage
	* Major Outage

## Requirements

* Zabbix 6.0 or Later (tested on Zabbix 7.2)
* Outbound access on TCP 443 from Zabbix Server to the target status page URL

## Import

1. Data Collection > Templates
2. Import
3. Upload Template

## Using the Template

1. Create a host 
1a. Hostname (Eg. Jira)
1b. Template: Atlassian Status Page
1c. Host Group (Eg. Applications)
2. Macros > Inherited and host macros
2a. {$STATUSURL} = Status Page url with trailing / (eg. https://www.githubstatus.com/)

## License
**MIT License**
