---
layout: post
title:  "Git Credential Manager Core Authentication"
date:   2021-11-02 12:00:00 -0400
categories: [GCM]
author: Brad Turner
---
#Authentication Failure

While connecting to an on-prem instance of Azure DevOps 2020 via a Windows 10 v20H2 virtual machine I ran into an issue where git commands would not prompt for user credentials.  Any git command executed would produce an ```fatal: Authentication failed for ...``` error.  After a bit of digging through the logs, I found that Git Credential Manager Core (GCM) was detecting that the on-prem instance of Azure DevOps supports Windows Integrated Authentication (WIA) and therefore instructing GCM to use WIA to supply user credtials.  Since the account I was using to log into the virtual machine was not a valid user account for the Azure DevOps instance the authentication failed.  So, how do we tell GCM to ignore WIA if it is detected for our on-prem instance and instead prompt for user credentials?  ```git config --global credential.myonpremserverinstance.com.allowWindowsAuth false```
