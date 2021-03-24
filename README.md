# HadoopConfiguration

Usecase:
Configure Hadoop and start cluster
services using Ansible Playbook


Changes required while using this playbook
1)Add master and slave ip and password inside inventory file.
Master must be one and slave can be multiple.
2) Inside configuration files go inside master_core_site.xml and slave_core_site.xml files and insert master ip in both .xml file instead of <master_ip> value.
3)If you doing this setup over cloud then inside master_core_site.xml replace <master_ip> value with 0.0.0.0 and inside slave_core_site.xml use master systems public ip.

Note: Python3 and Ansible must be installed inside main system.
