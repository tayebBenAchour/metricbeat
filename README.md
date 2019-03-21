Role Name
=========

Install and configure Metricbeat service


Role Variables
--------------

All variables you can find in default/main.yaml. To use this role you don't need configure anything, but to use them you need setup output, elasticsearch on logstash.
```yaml
es_metricbeat_output: 'elasticsearch'
es_metricbeat_output_elastic:
  - es1.example.com
  - es2.example.com
```
or
```yaml
es_metricbeat_output: 'logstash'
es_metricbeat_output_logstash:
  - ls1.example.com
  - ls2.example.com
```

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - metricbeat

License
-------

BSD

Author Information
------------------

Tomasz Baczynski
