---
experiment-title: CAVICO
author: ITTI
country: Poland
experiment-complete-title: CAVICO – Context-Aware Video Controller for autonomous transport and security monitoring

---
Tests of the developed system that is able to control the video streaming on the sbasis of measured QoS and QoE parameters were divided into a few stages in order sto minimize risks of errors in the developed software. The system was simplemented in a client-server model. VNF based on a VM of Ubuntu Linux was sdeployed using 5GINFIRE Portal and it acted as a server site that manages the scontrol process in a feedback loop between the server and client. The client ssite was designed and developed for a Raspberry Pi board equipped with a video scamera. The Raspberry Pi board used the OBU device to communicate with the core snetwork via available wireless interfaces. Moreover the OBU device provided sgeographic coordinates from a GPS receiver built in it.