---
title: Azure Monitoring Projects
date: 2024-10-25 13:40 +0200
categories: [projects,github,azure]
tags: [dashboard,rbac,automation]     # TAG names should always be lowercase
---

<div style="background-image: url('https://cdn.pixabay.com/photo/2019/03/18/13/58/heaven-4063166_1280.jpg'); 
            background-size: cover; 
            background-position: center; 
            width: 100%; 
            height: 300px;">
</div>

<br>
<br>



# Why Azure Monitoring?

A proposal came up recently at my current job to create a Dashboard for our Azure resources to provide a holistic view of what’s running in the cloud and the status of different resources. Although it won’t be my project, I couldn’t help but feel curious. So, I decided to create a mini-version of that dashboard in my spare time to gain experience and simply because I enjoy learning new technologies 😊.

# Azure Monitoring Projects

The idea is simple: I start with easier projects and gradually increase the difficulty. Each project builds on previous knowledge, providing a strong introduction to cloud monitoring and automation in Azure.

## Project 1: [CPU Usage Monitoring](https://github.com/madebydawid/azure-monitoring-projects/tree/main/Project%201%3A%20CPU-monitoring)

My first project focused on setting up monitoring and alerts for CPU usage on an Azure virtual machine. 

This project taught me the *basics of configuring CPU monitoring*, *setting thresholds*, and *sending email alerts*. It showed me how important it is to identify resource bottlenecks early, which is critical for maintaining system performance.

## Project 2: [RAM Monitoring](https://github.com/madebydawid/azure-monitoring-projects/tree/main/Project%202%3A%20RAM-monitoring)

In the second project, I tested monitoring available memory on a VM and set up automated actions. The *goal was to automate RAM monitoring and trigger an alert* when available memory dropped below a certain threshold. 

This project strengthened my skills in Azure Monitor and gave insights into setting up alerts that can automatically adjust resources as needed.

## Project 3: [Real-Time Dashboard for Multiple Resources](https://github.com/madebydawid/azure-monitoring-projects/tree/main/Project%203%3A%20Real-Time%20Dashboard%20for%20Multiple%20Azure%20Resources)

The final project was both the most challenging and rewarding. Here, I set up a real-time dashboard to monitor CPU, RAM, and network traffic across three virtual machines. Each VM had specific thresholds and configurations:

- **VM1 monitored CPU usage** and sent an email alert when usage exceeded 80%.
- **VM2 monitored available RAM** and sent a warning email when memory dropped below 20%.
- **VM3 monitored network traffic** and used an Azure Automation runbook to respond when traffic exceeded 200MB.

To simulate network traffic, I used [*iPerf3*](https://github.com/madebydawid/azure-monitoring-projects/blob/main/Project%203:%20Real-Time%20Dashboard%20for%20Multiple%20Azure%20Resources/images/vm2-sendingtovm3.jpg?raw=true) between VM2 and VM3. 
After configuring [an inbound security rule](https://github.com/madebydawid/azure-monitoring-projects/blob/main/Project%203:%20Real-Time%20Dashboard%20for%20Multiple%20Azure%20Resources/images/vm3-rbac-rule.jpg?raw=true) for TCP traffic on port 5201 and ensuring the right [Azure RBAC permissions](https://github.com/madebydawid/azure-monitoring-projects/blob/main/Project%203:%20Real-Time%20Dashboard%20for%20Multiple%20Azure%20Resources/images/RBAC-assignment.png?raw=true), the automation worked seamlessly. When the traffic limit was reached, the runbook triggered automatically and showed the status in real-time in the test pane – a major milestone for integrating monitoring and automation.

To send traffic between VM2 and VM3 with iPerf3 following steps were executed:

```bash
# Install iPerf3
sudo apt-get install iPerf3
```

```bash
# Set VM3 to act as a server
iPerf3 -s
```

```bash
# Send network traffic
iperf3 -c 20.240.193.196 -t 60 -b 220M -p 5201
```
-   -c = IP number
-   -t = Time to send traffic
-   -b = Amount of traffic
-   -p = Destination port

## What I Learned

This project gave me a deeper understanding of real-time monitoring and complex alert rules in Azure. It also offered insights into combining automation and security configurations to create efficient, self-sustaining systems. Overall it was an exciting project that had me using different resources to complete it!

## Next Steps

In the future I plan to explore log analytics in Azure. and see how advanced automation can be applied to additional resources.

---

>#### This and other projects can be found at my [GitHub](https://github.com/madebydawid).
---

//Cheers - Dawid