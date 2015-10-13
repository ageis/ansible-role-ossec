# ansible-role-ossec

Ansible role for setting up an OSSEC server and multiple agents.

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

Then run the role against both groups, `ossec_manager:ossec_agents`. 
See `examples/ossec.yml` for an example playbook. 

## License
MIT
