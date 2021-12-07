# ELK-stack
Ansible playbook for deploying a ELK cluster with 1 master and 2 worker nodes on a RedHat family environment

To run the playbook:

ansible-playbook --vault-id elk@vault-pass site.yml

- group_vars:  
Holds all role variables for servers defined in environments file.

Roles:

elasticsearch:  
This role configures and installs the elasticsearch cluster (1 master/vote & 2 master/data nodes)

filebeat:  
This role configures and installs filebeat

kibana:  
This role configures and installs kibana on master/vote node

kibana-dashboards:
This role configures the initial dashboards in kibana that come as default

filebeat:  
This role configures and installs filebeat

metricbeat:  
This role configures and installs metricbeat