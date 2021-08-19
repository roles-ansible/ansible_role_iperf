[![galay](https://raw.githubusercontent.com/roles-ansible/ansible_role_iperf/main/.github/galaxy.svg)](https://galaxy.ansible.com/do1jlr/iperf)
[![MIT License](https://raw.githubusercontent.com/roles-ansible/ansible_role_iperf/v1.0.0/.github/license.svg)](https://github.com/roles-ansible/ansible_role_iperf/blob/main/LICENSE)

 ansible_role_iperf
====================
Ansible role to install, run and configure a iperf3 server.


 variables
------------

| variable | default value | description |
| -------- | ------------- | ----------- |
| ``iperf__systemd_enable`` | ``true`` | enable and run or stop and mask the systemd iperf.service |
| ``iperf__options`` | ``'--server'`` | The option for the iperf3 Server |
| ``iperf__packages`` | ``iperf3`` | Packages to install by this role |
| ``iperf__package_state`` | ``present`` | package state. use latest for upgrading installed "{{ iperf__packages }}" |
| ``iperf__user`` | ``iperf`` | User that will run iperf3 as systemd service |
| ``iperf__group`` | ``iperf`` | Group for "{{ iperf__user }}" |
| ``submodules_versioncheck`` | ``false`` | Perform a optional simple versionscheck to prevent running a old version of this role *(recomended)* |

 DOCS
------
Have a look at https://iperf.fr/iperf-doc.php for iperf Dokumentation

 Testing
----------
Linting of this role is tested using github actions. If you know a great way to test systemd stuff via github-actions please leave a note!
