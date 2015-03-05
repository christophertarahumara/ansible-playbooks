# Hupp ansible-playbooks

where we put our ansible playbooks

## elasticsearch

From [https://github.com/Traackr/ansible-elasticsearch](https://github.com/Traackr/ansible-elasticsearch)

Not modified, only variables are used to configure the installation.

Command used to install: `ansible-playbook -i hosts elasticsearch.yml -K`

## logstash

From [https://github.com/valentinogagliardi/ansible-logstash](https://github.com/valentinogagliardi/ansible-logstash)

Modified `outputs.j2`, `filters.j2` and `inputs.j2` because it felt clearer
to have the json conf in real json files instead of in the Ansible yml.

Command used to isntall: `ansible-playbook -i hosts logstash.yml -K`
