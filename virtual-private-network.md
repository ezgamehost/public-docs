---
title: Private Virtual Networking
description: 
published: true
date: 2025-12-24T06:28:10.101Z
tags: 
editor: markdown
dateCreated: 2025-12-24T06:28:10.101Z
---

## Core Concepts

- Networks: Networks are top level logical encapsulations of networking resources.

- Subnets: Subnets are individual virtual layer 2 domains to place networked devices into (ie: Compute Instances).

- Routers: Routers are virtual software based appliances that act as a gateway to forward traffic between subnets.

- Ports: Ports are connections different resources create with the subnet. Each port would be assigned one or more IP address(es).

- Floating IP: These are publically routable IP addresses that individually map to a internal resource. These are independently managed away from each individual instance thus are not affected by instance lifecycle.
