---
title: Experiments
subtitle: 5G-CAGE
experiment-title: 5G-CAGE
author: University of Murcia
country: Spain
experiment-complete-title: 5G-enabled Context and situational Awareness detection with machine learninG techniques of city objects in Experimental vertical instances (5G-CAGE)

---
# Title
5G-enabled Context and situational Awareness detection with machine learninG techniques of city objects in Experimental vertical instances (5G-CAGE)

# Organization
University of Murcia, Spain – http://www.um.es/english

# Experiment description
5G networks are opening up a wide range of new opportunities for the Public Safety industry. Video surveillance and new generation Public Safety Networks (PSN) are intrinsically tied together, as the number of distributed devices such as cameras, recorders and sensors are increasing in Smart Cities. With 5G, the amount of data available for public safety applications is expected to increase tremendously, mostly in terms of video/audio streaming, location information and context-awareness. The application of intelligence mechanisms to detect certain situations or city objects (e.g. license car plates in which PSN operators are interested in quickest reaction to terrorist attacks, crimes or natural disasters) becomes a great challenge targeting Big Data analytics.

In the above context, 5G-CAGE aims at deploying a City Safety solution as a new NFV Network Service into 5GINFIRE Experimental Vertical Instance (EVI), called City Object Detection (CODet), for automatic detection and location of certain city elements and objects. Specifically, 5G-CAGE provides a CODet VxF to detect license car plates via advanced Computer Vision and Machine Learning algorithms, by means of the monitoring and analytics of video streams collected from cameras equipped in vehicles connected to the Smart City infrastructure. The 5G-CAGE City Safety solution has been exercised and successfully tested in the 5GINFIRE IT-Av Automotive Environment belonging to the 5GINFIRE project ecosystem.

The 5G-CAGE architecture is briefly illustrated below. The OBU connectivity capabilities are mainly through 4G and 802.11p to communicate with the 5GINFIRE infrastructure –where the 5G-CAGE CODet VxF is deployed at the IT-Av Cloud– through the Road-Side Units (RSU) or the Cloud Radio Access Networks (C-RAN). The GPS element in the OBU provides location data and the Wi-Fi link is used for in-vehicle connectivity, specifically with the In-Car Node Processor equipped with the video streaming camera.


![Cage 1](https://5ginfire.eu/wp-content/uploads/2019/06/cage1.jpg)


The figure shows that a registered license car plate has been detected in the Smart City, specifying the place extracted from the GPS coordinates, the date and time of the precise time of detection, the confidence of the detection result (around 90%) and an image of the license car plate after being cropped from the original complete frame so as to preserve privacy issues. An embedded web frame is also shown to review the car location on the map.

## Results

As aforementioned, 5G-CAGE has been tested in the 5GINFIRE IT-Av Automotive Environment so as to assess performance in terms of precision detecting license car plates as well as the volume of network traffic required by the CODet VxF for operation. The 5G-CAGE City Safety solution has been tested under real driving conditions by using a single vehicle equipped with a video streaming camera, configured with a resolution of 1280×720, going around a circuit with six license car plates. The next figure shows the experimental results in processing time.

The test output has 60 results, taking into account that in the vehicle route the same license car plates appear in different frames. The average processing time is 473ms, where the time to analyse each plate is around 55ms (in red). As shown, the detection stage is the most time-consuming phase (in green) and presents time spikes depending on the complexity of the frame. On the other hand, it is worth noting that the confidence in detection is 84.11% on average, a very consistent value with the experiment conditions.

On the other hand, the next figure shows the performance measure regarding the amount of network traffic required by the CODet VxF to gather video streams from a single vehicle in the IT-Av Automotive Environment testbed, in particular from its In-Car Node Processor. This plot displays the rate of data across a network connection, in particular regarding the data plane network interface connecting the vehicle with the 5GINFIRE platform.

![Cage 2](https://5ginfire.eu/wp-content/uploads/2019/06/cage2.jpg)

167.77 KB/s on average is being displayed, indicating that the volume of traffic would be an issue to consider in real automotive scenarios with a greater number of vehicles in motion. However, this potential traffic congestion could be addressed by decoupling the CODet detection functions and transferring part of the solution to each vehicle’s OBU. In this way, only results of the detection of each frame, if any, will be sent to the CODet VxF for further analysis, thus reducing the amount of traffic in video streaming delivery.

## Conclusions

5G-CAGE presents a City Safety solution to supply PSN operators (e.g. police officers) with an intelligent mechanism capable of identifying specific city objects such as license car plates in an automotive scenario within a Smart City ecosystem, through advanced Computer Vision and Machine Learning algorithms. The 5G-CAGE City Object Detection (CODet) VxF has been successfully deployed and tested in the 5GINFIRE EVI environment, specifically using the IT-Av Automotive Environment and the 5TONIC Open 5G Lab. The experimental results obtained have confirmed the feasibility of the CODet VxF of being implemented and deployed in a Smart City ecosystem. Although potential traffic congestion may appear in similar conditions, a solution by decoupling the CODet VxF functionality towards the edge computing has been described to mitigate the network problems that may arise. As further research, the 5G-CAGE CODet VxF functionalities could be extended to support other problems raised in emergency settings, speeding up response time of first responders in public safety interventions (e.g. natural disasters such as earthquakes or wildfires).