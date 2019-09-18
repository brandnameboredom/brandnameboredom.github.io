---
layout: post
title:  "Kubevirt"
date:   2019-09-16 12:00:00 -0400
categories: [Kubevirt, VM, Kubernetes]
author: Brad Turner
---

Recently I've come accross a legacy application deployed within VMs and was asked what the migration strategy should in order to convert the application over to containers which could be managed by a container orchestration technology like Kubernetes (specifically OpenShift).  So, I decided now was as good a time as any to take a look at kubevirt.  To be honest, this had been on my list of "Go check this out.  This group is doing some pretty amazing stuff" but I hadn't found/made the time to investigate.  

First Impressions...Whoa.

The ability to manage VMs as native Kubernetes resources including horizontal scaling and quota limitations seems like exactly what this application needs to start benefitting from what Kubernetes offers while rearchitecting to take full advantage of the technology.  Obviously there are inherent costs associated with the "lift and shift" method of deployment but since this would be deployed within an on-prem cloud and the cost of infrastructure is not prohibitive in this environment this seems like a perfect fit.  

