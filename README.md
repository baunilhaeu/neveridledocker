# neveridleDocker
This is the implementation of layou233's amazing NeverIdle script for Easypanel/docker on ARM64 Oracle Cloud Instances.

## Why
Recently, some Oracle Cloud Free Tier users received an email stating that their compute instances were identified as idle and would be stopped in one week. Since Oracle Free Cloud is by far the best offer for test servers, some users may not want to lose their machines.

This script is made to run on Easypanel, a docker-based control panel, and helps to avoid the instance from being considered idle, thus preventing Oracle from deleting your machine. It makes your CPU waste 20% of processor power on a very low priority, which means that it will only waste if other more important processes are not using the machine. It also wastes your 2GB of memory and uses a speed test to consume about 20% of network, all in a docker image. Therefore, you don't have to use the screen attach and detach solution suggested on the layou233 solution.

## Installation
To install the script on Easypanel, create a new app, add this GitHub address, and deploy it.
![image](https://github.com/baunilhaeu/neveridledocker/blob/main/ep-git-neveridle.png)
