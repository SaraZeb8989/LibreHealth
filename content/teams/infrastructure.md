+++
title = "LibreHealth Infrastructure Team"
+++
The LibreHealth Infrastructure Team is responsible for maintaining the infrastructure
which LibreHealth relies on. Part of this requires that we have consistent monitoring/alerting
if systems are misbehaving or become unavailable.

# Services provided to us free as an Open Source organization
## Datadog

![datadog](https://app.datadoghq.com/event/icon/monitor_alert.png)

We are very gracious to [Datadog](https://datadoghq.com) for providing
use of their service free of charge through their [open source program](https://www.datadoghq.com/partner/open-source/).

### About Datadog
Datadog is a cloud-based service which provides infrastructure monitoring. We utilize ansible to provision nearly all servers and used the [official ansible role](https://github.com/DataDog/ansible-datadog) to install the datadog agent, but they have an official [Puppet module](https://github.com/DataDog/puppet-datadog-agent) and [Chef cookbook](https://github.com/DataDog/chef-datadog) as well. If you're one of those people, you can also install their agent manually.

### How we use it
We currently monitor the following: memory usage (take note that free memory in linux [is not what you think it is](http://www.linuxatemyram.com/)), disk utilization, swap, host down, and docker daemon up. These We also monitor nginx and apache as well.

We would like to set up public dashboards so that we can see at a glance, the health of our infrastructure, and will have links here when those are created.
