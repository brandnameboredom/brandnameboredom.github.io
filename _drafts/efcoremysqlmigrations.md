---
layout: post
title:  "Mysql DateTime Default EF Core"
date:   2016-06-20 12:00:00 -0400
categories: [entity framework, dotnetcore, database, migrations, mysql]
author: Brad Turner
---

## Designating a default value for a DateTime column in MySql 8 using [Entity Framework Core]

MySQL version 5.6 introduced [automatic initialization and updating for TIMESTAMP and DATETIME].  So, when adding a "CreatedDate" and "LastModifiedDate" property to a model I was working on, I thought I would created the relatively simple database migration to set the value of these columns to the current date and time upon creation.  Turns out what I thought would be "relatively simple" is, in fact, not at all...

Ok, Step 1: Update my model

[Entity Framework Core]: https://docs.microsoft.com/en-us/ef/core/
[automatic initialization and updating for TIMESTAMP and DATETIME]: https://dev.mysql.com/doc/refman/5.6/en/timestamp-initialization.html
