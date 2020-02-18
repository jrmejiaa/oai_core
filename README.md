# OpenAirInterface (OAI)
The purpose of this wiki is to include all the important information about the use of the interface Open Air Interface to make a EPC Component, because the project has different places of relevant documentation to solve this problem. Here it would be include the useful information about how install all the needed packages and examples of how it should be used. 

## 1. Introduction
OpenAirInterfaceTM (OAI) wireless technology platform is a flexible platform towards an open LTE ecosystem. The platform offers an open-source software-based implementation of the LTE system spanning the full protocol stack of 3GPP standard both in E-UTRAN and EPC. It can be used to build and customize  a LTE base station (OAI eNB), a user equipment (OAI UE) and a **core network (OAI EPC) on a PC**. The OAI eNB can be connected either to a commercial UEs or OAI UEs to test different configurations and network setups and monitor the network and mobile device in real-time. In addition, OAI UE can be connected to eNB test equipment (CMW500) and some trials have been successively run with commercial eNB in December 2016.

OAI is based on a PC hosted software radio frontend architecture. With OAI, the transceiver functionality is realized via a software radio front end connected to a host computer for processing. OAI is written in standard C for several real-time Linux variants optimized for IntelTM x86 and ARMTM processors and released as free software under the OAI License Model. OAI provides a rich development environment with a range of built-in tools such as highly realistic emulation modes, soft monitoring and debugging tools, protocol analyzer, performance profiler, and configurable logging system for all layers and channels.

Towards building an open cellular ecosystem for flexible and low-cost 4G/5G deployment and experimentations, OAI aims at the following objectives:

* Open and integrated development environment under the control of the experimenters.
* On the network side: Fully software-based network functions offering flexibility to architect, instantiate, and reconfigure the network components (at the edge, core, or cloud using the same or different addressing space).
* On UE side : Fully software-based UE functions which can be used by modem designers with upgrading and/or developing LTE and 5G advanced features.
* Playground for commercial handsets as well as application, service, and content providers.
* Rapid prototyping of 3GPP compliant and non-compliant use-cases as well as new concepts towards 5G systems ranging from M2M/IoT and software-defined networking to cloud-RAN and massive MIMO.

### Evolved packet core network features:

* MME, SGW, PGW and HSS implementations. OAI reuses standards compliant stacks of GTPv1u and GTPv2c application protocols from the open-source software implementation of EPC called nwEPC.
* NAS integrity and encryption using the AES and Snow3G algorithms.
* UE procedures handling: attach, authentication, service access, radio bearer establishment.
* Transparent access to the IP network (no external Serving Gateway nor PDN Gateway are necessary). Configurable access point name, IP range, DNS and E-RAB QoS.
* IPv4 and IPv6 support.

![OAI_Stack](https://www.openairinterface.org/wp-content/uploads/2015/08/oai_stack.png)

OAI platform can be used in several different configurations involving commercial components to varying degrees:

* Commercial UE ↔ Commercial eNB + OAI EPC
* Commercial UE ↔ OAI eNB + Commercial EPC
* Commercial UE ↔ OAI eNB + OAI EPC
* OAI UE ↔ OAI eNB + OAI EPC
* OAI UE ↔ OAI eNB + Commercial EPC
* OAI UE ↔ Commercial eNB + Commercial EPC

## 2. Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system. Please go to the [Installation Process](https://github.com/jrmejiaa/EVERIS_OAI/wiki/Getting-Started) to see step by step. 

## 3. Deployment
The running application after the installation can be seen here in the [Running EPC](https://github.com/jrmejiaa/EVERIS_OAI/wiki/Deployment)

## 4. License
The source code is mainly written under the [Apache V2.0 License](http://www.apache.org/licenses/LICENSE-2.0). The text for Apache V2.0 License is also available under LICENSE file in the same directory. For more details on third party software, please read the NOTICE file in the same directory.

