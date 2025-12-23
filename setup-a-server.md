---
title: Setup a New Server
description: Setup a new server on the EZ Game Host platform 
published: true
date: 2025-12-23T10:18:25.486Z
tags: 
editor: markdown
dateCreated: 2025-12-23T09:59:52.837Z
---

### Prerequisite
To get started with setting up a cloud server on the platform, you first need an activated account with the EZ Game Host Cloud platform. To see how, check out [Setup a Cloud Account](/setup-cloud-account).

###

First, go to the server tab of the dashboard. ![screenshot_2025-12-23_at_1.55.46_am.png](/screenshot_2025-12-23_at_1.55.46_am.png)

We currently have prepared images for various popular distribution of Linux including Debian, Ubuntu, CentOS, Rocky Linux, Fedora and Alpine. We will also be gradually rolling out custom images for various applications. 

The EZ Game Host Cloud is currently available in us-west-1 region only. However, we are constantly expanding. If you are interested in a different region, email [support](mailto:support@ezgamehost.com) with your request and we will actively expand for your needs if possible.

After selecting the image, next select the hardware to utilize.

We currently have two class of hardware available, General Purpose and High Performance instances. General Purpose instances run on Xeon golds which are optimized for multi threaded applications. These are more economical and would work well for web applications, databases, etc that can multi thread workloads and generally don't expect too much traffic.

We also provide High Performance Compute instances. These are latest generation Ryzen 9 9950X servers with high speed DDR5 memory. These tend to be most costly. However, they can go up to 4.7ghz on all cores. These are optimized for extremely single threaded workloads, like running game servers etc.

![screenshot_2025-12-23_at_2.13.10_am.png](/screenshot_2025-12-23_at_2.13.10_am.png)

After selecting the instance type, make sure to create a root volume so it will be stored on the platform block store instead of per instance instance storage.

Also, make sure to attach a network interface to public. This will provide internet bound access. 

If you are interested in BYoIP via announcing your own ASN or utilizing our ASN to announce your IP space. [Contact Us](mailto:support@ezgamehost.com)

![screenshot_2025-12-23_at_2.16.44_am.png](/screenshot_2025-12-23_at_2.16.44_am.png)

Next, upload your SSH key to the platform. If you don't know how to generate a SSH key. Check out our article on [SSH](/en/what-is-ssh).

Also, make sure to create a security group to allow public access to your instance.

At last, choose to good name for your instance so you won't forget about what the instance does many months down the line!