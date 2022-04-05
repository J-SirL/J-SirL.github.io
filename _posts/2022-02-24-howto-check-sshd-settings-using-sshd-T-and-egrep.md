---
title: HowTo check sshd settings using sshd -T and egrep
date: 2022-02-24
categories: [Linux, HowTo]
tags: [ssh, linux, bash, egrep, settings, check, quicktips, howto]     # TAG names should always be lowercase
---



# HowTo: Check the sshd settings using sshd -T and egrep

By combining egrep with sshd -T you can simply check the settings of sshd.


```bash
sudo sshd -T | egrep -i 'allowusers|passwordauth|permitroot'
```

Example output

![example of sshd settings](/images/pages/sshd-t-egrep.png)

[Man pages for SSHD](2022-02-25-sshd-man-pages.md)

    sshd -T  Extended test mode.  Check the validity of the configuration
             file, output the effective configuration to stdout and then exit.
             Optionally, Match rules may be applied by specifying the connec‐
             tion parameters using one or more -C options.