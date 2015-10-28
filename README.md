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

### Vars
Declare `ossec_directories_to_watch` as a list to provide a custom set
of directories to watch. Regardless of whether `ossec_directories_to_watch`
is set, a few critical dirs will be monitored for changes:

  * `/bin`
  * `/etc/`
  * `/sbin/`
  * `/usr/bin`
  * `/usr/sbin`

## License
MIT
