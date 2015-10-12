# OSSEC agent and server

Ansible roles for setting up an OSSEC server and multiple agents.

## Usage
Populate your hosts/inventory file with the OSSEC server and a hostgroup for its clients like so:

```
[ossec_manager]
monitoring.example.com

[ossec_agents]
web.example.com
db.example.com
mail.example.com
```
