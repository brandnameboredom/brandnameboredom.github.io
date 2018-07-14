---
layout: post
title:  "AWS Curiosities"
date:   2018-07-14 12:00:00 -0400
categories: [AWS]
author: Brad Turner
---

# S3

## Cross Region Replication

When two s3 buckets are configured for cross region replication and a deletion marker is created for a file in one of the s3 buckets it is replicated over to the linked s3 bucket.  However, if the deletion marker is itself deleted, that action is not replicated. Hmm.
