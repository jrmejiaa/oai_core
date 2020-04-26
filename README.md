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
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### 2.1. Prerequisites
* Knowledge about Communications and its protocols to work with a 4G LTE and 5G Network. There is a section in this wiki who can help with this requirement. If you need, please go to [Should Know](https://github.com/jrmejiaa/EVERIS_OAI/wiki/Should-Know)
* **Hardware Requirements:** According to [OAI Requirements Site](https://gitlab.eurecom.fr/oai/openairinterface5g/wikis/OpenAirSystemRequirements) it is necessary a PC who has an Intel processor to work the eNB or UE targets. This requirement is due to optimized DSP functions
which make heavy use of integer SIMD instructions (SSE, SSE2, SSS3, SSE4, and AVX2). It recommends to work with the Family `Generation 3/4/5/6 Intel Core i5,i7`.
* **Software Requirements:** The OpenAir-CN EPC component should work on a Ubuntu Bionic according to the last information in the wiki [OAI EPC Instalation](https://github.com/OPENAIRINTERFACE/openair-cn/wiki/OpenAirSoftwareSupport), besides it needs some kernel changes to work properly, therefore it is recommended to work in a virtual machine. However for the eNB and UE OAI, it needs a Ubuntu Xenial with an specific low-latency kernel, those steps are explained in the Gitlab of the project. Those steps are found in the UE and eNB installation process. 

### 2.2. Installing

* Please go to the [EPC Installation Process](https://github.com/jrmejiaa/EVERIS_OAI/wiki/EPC-Installation) to see step by step to make your EPC machine working. 

* Please go to the [UE+eNB with NFAPI Simulator](https://github.com/jrmejiaa/EVERIS_OAI/wiki/UE-and-eNB-with-L2-NFAPI-Simulation) to see step by step to make your UE and eNB working.

## 3. Deployment
It uses the EPC Core of OAI with the UE+eNB to make a deployment and to attach a UE with the EPC and see its behavior. In this link you can see here [Deployment OAI using NFAPI Simulator](https://github.com/jrmejiaa/EVERIS_OAI/wiki/Deployment-OAI-using-NFAPI-Simulator)

## 4. License
The source code is mainly written under the [Apache V2.0 License](http://www.apache.org/licenses/LICENSE-2.0). The text for Apache V2.0 License is also available under LICENSE file in the same directory. For more details on third party software, please read the NOTICE file in the same directory.
