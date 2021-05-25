# What Is Merlin?

## Merlin

### Automated State Capture and Documentation

#### Capture Network State and Transform it into Business-Ready Documentation
| Filetype | Extension | Description |
| -------- | --------- | ----------- |
| Comma-Separated Values | .csv | Excel-ready, searchable, sortable, filterable, spreadsheet |
| Markdown | .md | Browser ready, lightweight, portable, Markdown file |
| Hyper-Text Markup Language | .html | Web-ready HTML file |
| Mind Map | .html | Interactive, zoom / collapse, dynamic, HTML Mind Map rendered from the Markdown |
| Network Graph | .html | Interactive, hyper-connected, HTML network graph based on the NETJSON standard |

#### CLI
##### Currently Tested Platforms
| IOS | Platform |
| --- | -------- |
| IOS | Cisco Catalyst 2960 |
| IOS | Cisco Catalyst 3560 |
| IOS | Cisco Catalyst 3750 |
| IOS | Cisco Catalyst 6500 |
| IOS | Cisco Catalyst ISR 891FW |
| IOS-XE | Cisco Catalyst 3850 |
| IOS-XE | Cisco Catalyst 9300 |
| IOS-XE | Cisco Catalyst 4500 |
| IOS-XE | Cisco Catalyst ISR 4400 |
| IOS-XE | Cisco CSR1000v |
| NXOS | Cisco Nexus 9000 |
| NXOS | Cisco Nexus 7000 |
| NXOS | Cisco Nexus 5000 |
| NXOS | Cisco Nexus 2000 FEX |
| JUNOS | Juniper 17 / 18 / 19 |

##### Current pyATS Functions
| pyATS | Function | 
| --- | -------- |
| learn() | ACL |
| learn() | ARP |
| learn() | BGP |
| learn() | CONFIG |
| learn() | DOT1X |
| learn() | INTERFACE |
| learn() | LLDP |
| learn() | NTP |
| learn() | OSPF |
| learn() | PLATFORM |
| learn() | ROUTES |
| learn() | STP |
| learn() | VLAN |
| learn() | VRF |
| parse() | show access lists |
| parse() | show access sessions |
| parse() | show access session interface {{ interface }} detail |
| parse() | show authentication sessions |
| parse() | show authentication session interface {{ interface }} detail |
| parse() | show cdp neighbors |
| parse() | show bgp process VRF all |
| parse() | show bgp sessions |
| parse() | show cdp neighbors details |
| parse() | show environment all |
| parse() | show etherchannel summary |
| parse() | show interfaces |
| parse() | show interfaces status |
| parse() | show interfaces trunk |
| parse() | show inventory |
| parse() | show ip arp |
| parse() | show ip arp vrf {{ vrf }} |
| parse() | show ip interface brief |
| parse() | show ip ospf |
| parse() | show ip ospf database |
| parse() | show ip ospf interface |
| parse() | show ip ospf neighbor |
| parse() | show ip ospf neighbor detail |
| parse() | show ip route |
| parse() | show ip route vrf {{ vrf }} |
| parse() | show issu state detail |
| parse() | show mac address-table |
| parse() | show ntp associations |
| parse() | show power inline |
| parse() | show version |
| parse() | show vlan |
| parse() | show vrf |
| parse() | show vrf all detail | 
| parse() | show vrf all interface |


#### REST-API
##### Currently Tested Platforms
| Platform | Description |
| -------- | ----------- |
| BIG-IP | Any F5 |
| ISE | Cisco Identity Services Engine External RESTFul Service (ERS) |
| ISE | Cisco Identity Services Engine Monitoring and Troubleshooting (MnT) |
| Cisco.com | Cisco Serial 2 Info |
| Cisco.com | Cisco Recommended Release |

##### Current REST Functions
| Platform | API |
| -------- | --- |
| ISE ERS | Administrators |
| ISE ERS | Allowed Protocols |
| ISE ERS | Authorization Profiles |
| ISE ERS | dACLS |
| ISE ERS | Endpoint Groups |
| ISE ERS | Identity Groups |
| ISE ERS | Network Devices |
| ISE MnT | Total Active Sessions |
| ISE MnT | Active Sessions |
| ISE MnT | MAC Session Details |
| F5 BIG-IP | Virtual Servers |
| F5 BIG-IP | SSL Certificates

#### SharePoint Integration
##### POST CSV and other files directly in to SharePoint document library via REST API

### Security Posture

#### Access-Lists
| Platform | Features | Description | 
| -------- | -------- | ----------- |
| IOS-XE | learn('acl') | Learn and transform ACL configurations |
| IOS-XE | parse('show acccess lists') | Learn and transform ACL configurations |

#### 802.1x
| Platform | Features | Description |
| -------- | -------- | ----------- |
| IOS-XE | learn('dot1x') | Learn and transform 802.1x configurations |
| IOS-XE| parse('show access session') | Learn and transform all current access sessions |
| IOS-XE| parse('show access session interface {{ interface }} detail') | Learn and transform granular per-interface access sessions |
| IOS-XE| parse('show authentication session') | Learn and transform all current authentication sessions |
| IOS-XE| parse('show authentication session interface {{ interface }} detail') | Learn and transform granular per-interface authentication sessions |
| ISE ERS | Authorization Profiles | Learn and transform Authorization Profiles |
| ISE ERS | dACLS | Learn and transform dACLS |
| ISE MnT | Total Active Sessions | Learn and transform all Total Active Authentication Sessions | 
| ISE MnT | Active Sessions | Learn and transform all Active Authentication Settings | 
| ISE MnT | MAC Session Details | Learn and transform per-MAC granular details |

#### Identity Services Engine
| Platform | Features | Description |
| -------- | -------- | ----------- |
| ISE ERS | Allowed Protocols | Learn and transform Allowed Protocols |
| ISE ERS | Endpoint Groups | Learn and transform Endpoint Groups |
| ISE ERS | Identity Groups | Learn and transform Identity Groups | 
| ISE ERS | Network Devices | Learn and transform Network Devices |

#### F5
| Platform | Features | Description |
| -------- | -------- | ----------- |
| F5 BIG-IP | SSL Certificates | Learn and transform all F5 SSL Certificate details |

#### Cisco Product Security Incident Reponse Team (PSIRT)
##### Automatically Assess the Security Posture by Sending Each PID to the PSIRT REST API at Scale

#### Cisco Recommended Release
##### Automatically Assess the Cisco Recommended Release by Sending Each PID to the REST API

### ChatBots
#### Automatically Send Network State Information in Instant Messages to Various Channels
| Platform |
| -------- |
| Cisco WebEx |
| Discord |
| Slack |
| Teams |

### VoiceBots
#### Automatically transform Network State Information into MP3 Files using Cloud Text-To-Speech Services 
| Platform |
| -------- |
| Google Text-To-Speech |
| Microsoft Azure Text-To-Speech |
| 3rd Party Text-To-Speech |

#### Automatically *Phone* *ANY* Number in the World to Deliver the MP3 Message as a Phone Call
| Platform | 
| -------- |
| Twilio |

## Lancelot

### Automated Intent-Based, Idempotent, SSH and REST API Configuration Management

#### Infrastructure as Code

##### YAML Data Model
| Abstracted Intent File |
| ---------------------- |
| Platform Agnostic Abstracted Representation of Intent as YAML |

##### Jinja2 Templates
| IOS / IOS-XE / NXOS CLI Configuration Stanza Templates |
| ------------------------------------------------------ |
| REST API JSON Templates |

##### Intended Configuration
| Dynamically Compiled Intended Configurations |
| -------------------------------------------- |
| CLI - IOS / IOS-XE / NXOS - Idempotent Imperative Cisco CLI Configurations Pushed using pyATS device.configure() |
| REST API - IOS-XE / NXOS - Idempotent Declarative Cisco REST API Configurations Pushed using Python requests.put() |

##### Differential 
| Dynamic State Change Tracking |
| ------------------------------------------------------------------------------------------------- |
| Original (Pre-Change) State Dynamically Compared (pyATS Diff) With New Golden Image (Post-Change) |

## Excalibur

### Automated Asset Management