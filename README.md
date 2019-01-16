# An Ansible role to setup and configure the Nginx integration for the Datadog Agent
The [Datadog.datadog role][] maintained by Datadog is great, but it does not attempt to configure services for monitoring.
In order to have it configure multiple integrations, you
would either have to:
 * duplicate your configs a lot
 * do tricky things with Ansible variables
which you shouldn't be doing and aren't worth your time.

This role provides an alternate way to setup a target machine and its Datadog agent to monitor Nginx.

## Installation

It is strongly recommended that the [Datadog.datadog role][] is used to install the agent.

> *NOTE* This integration requires Nginx be configured to expose a stats endpoint over http.
Setup instructions can be found at: https://docs.datadoghq.com/integrations/nginx/

Consult this role's [defaults](defaults/main.yml) for variables names.

[Datadog.datadog role]: https://github.com/DataDog/ansible-datadog
