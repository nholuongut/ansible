# nholuongut - Ansible

![](https://i.imgur.com/waxVImv.png)
### [View all Roadmaps](https://github.com/nholuongut/all-roadmaps) &nbsp;&middot;&nbsp; [Best Practices](https://github.com/nholuongut/all-roadmaps/blob/main/public/best-practices/) &nbsp;&middot;&nbsp; [Questions](https://www.linkedin.com/in/nholuong/)
<br/>

<!-- INDEX_START -->

- [Quick Ansible Doc](#quick-ansible-doc)
- [Ansible Inventory](#ansible-inventory)
- [Ansible Playbooks](#ansible-playbooks)
  - [Check Diff, Then Run](#check-diff-then-run)
  - [Install Prometheus](#install-prometheus)
  - [Install Node Exporter](#install-node-exporter)
- [More Core Repos](#more-core-repos)
  - [Knowledge](#knowledge)
  - [DevOps Code](#devops-code)
  - [Containerization](#containerization)
  - [CI/CD](#cicd)
  - [DBA - SQL](#dba---sql)
  - [DevOps Reloaded](#devops-reloaded)
  - [Templates](#templates)
  - [Misc](#misc)

<!-- INDEX_END -->

## Quick Ansible Doc

See the [Ansible](https://github.com/nholuongut/knowledge-base/blob/main/ansible.md) page in
the [nholuongut/knowledge-base](https://github.com/nholuongut/knowledge-base) repo.

## Ansible Inventory

A template of a quick easy static Ansible inventory is here:

[inventory.ini](inventory.ini)

More advanced dynamic inventories that populate by querying things like cloud providers can be used via
[plugins](https://docs.ansible.com/ansible/latest/plugins/inventory.html).

## Ansible Playbooks

Quickly install to a given host using `-i <hostname>,` with the trailing comma
to let Ansible know it is an inline host list not an [inventory.ini](inventory.ini) file.

### Check Diff, Then Run

Find a playbook you want, then run a dry run `--check --diff` to see what it would do,
check your SSH config is set up with the right AWS pem keys etc:

```shell
ansible-playbook -i inventory.ini path/to/playbook.yml --check --diff
```

If it look ok, then run it:

```shell
ansible-playbook -i inventory.ini path/to/playbook.yml
```

### Install Prometheus

```shell
ansible-playbook -i localhost, prometheus/playbook.yml
```

### Install Node Exporter

```shell
ansible-playbook -i localhost, prometheus_node_exporter/playbook.yml
```

# 🚀 I'm are always open to your feedback.  Please contact as bellow information:
### [Contact ]
* [Name: nho Luong]
* [Skype](luongutnho_skype)
* [Github](https://github.com/nholuongut/)
* [Linkedin](https://www.linkedin.com/in/nholuong/)
* [Email Address](luongutnho@hotmail.com)
* [PayPal.me](https://www.paypal.com/paypalme/nholuongut)

![](https://i.imgur.com/waxVImv.png)
![](Donate.png)
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/nholuong)

# License
* Nho Luong (c). All Rights Reserved.🌟