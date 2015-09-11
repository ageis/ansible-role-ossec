# OSSEC agent and server

Ansible roles for setting up an OSSEC agent and server

## Usage
Populate hostgroups for the OSSEC server and its clients.

```
[ossec-manager]
monitoring.example.com

[ossec-agents]
web.example.com
db.example.com
mail.example.com
```
