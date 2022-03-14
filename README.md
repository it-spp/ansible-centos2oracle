# Playbook to switch from CentOS to Oracle Linux

This playbook is designed for easy switch the CentOS instances to Oracle Linux  
with a simple check for free mount points space.  
It is based on https://github.com/oracle/centos2ol.

## Before you start

**IMPORTANT:** this  playbook is not designed to handle all possible configurations.  
Please ensure you have a **backup** of the systems before you start.

## Usage
1. Clone this repository.
2. Modify ansible-centos2oracle.yaml:  
Replace **remote_user** and **/home/test/** with your values.  
You can also add similar checks for your mount points.
3. Modify inventory: Replace values with your values (IP's or hostnames).
4. Run the playbook: ansible-playbook -i inventory migrate-centos2oracle.yaml.