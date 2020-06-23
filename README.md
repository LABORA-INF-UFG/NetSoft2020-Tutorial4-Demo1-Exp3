# NetSoft2020-Tutorial4-Demo1-Exp3

This project aims to provide a set of tools through which it is possible to deploy the mobile network that makes up the [Software Radio Systems LTE](https://www.srslte.com/), as illustrated by the following image.
<p align="center">
    <img src="images/demo1-exp3.png"/> 
</p>

In this demo, the elements of [Software Radio Systems LTE](https://github.com/srsLTE/srsLTE) compose of RAN and core of 4G. The main goal of this experiment is to demonstrate a connection between UE in hardware (conventional cell phone), RAN in hardware (SDR - Software-Defined Radio) and software, and EPC core implemented in software.

The minimum hardware requirement and software to run this experiment is shown in the figure below.
<p align="center">
    <img src="images/demo1-exp3-hw-sw.png"/> 
</p>
For this experiment, we assume that the machine have full access to the internet.

# 1 Installation tools
We need two tools to run this experiment, _Git_ and _Docker_

To install _Git_ run the following command:
```
sudo sudo apt-get install git-all
```

To install _Docker_ run the following command:
```
sudo apt-get install docker-ce docker-ce-cli containerd.io (preciso checar. Precisa o compose?)
```

 After, we can clone the **NetSoft2020-Tutorial4-Demo1-Exp3 project**:
```
git clone https://github.com/LABORA-INF-UFG/NetSoft2020-Tutorial4-Demo1-Exp3.git
```

# 2 - Build and running srsLTE images

To build the eNB and EPC images use the follow command: 
```
sudo docker build -t xxxx .
```

To run the images  use the follow command: 
```
sudo docker-compose up -d
```