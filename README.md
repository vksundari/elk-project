# elk-project

## Project Activities
1. Create a new vNet in Azure in a different region, within the same resource group.
2. Create a peer-to-peer network connection between their vNets.
   a. Create a new VM in the new vNet that has 2vCPUs and a minimum of 4GiB of memory.
   b. Add the new VM to Ansible’s `hosts` file in their provisioner VM.
3. Create an Ansible playbook that installs Docker and configures an ELK container.
4. Run the playbook to launch the container.
5. Restrict access to the ELK VM.

## Filebeat and Metricbeat activities
 1. Navigate to the ELK server’s GUI to view Filebeat installation instructions.
 2. Create a Filebeat configuration file.
 3. Create an Ansible playbook that copies this configuration file to the DVWA VMs and then installs Filebeat.
 4. Run the playbook to install Filebeat.
 5. Confirm that the ELK stack is receiving logs.
 6. Install Metricbeat as a bonus activity.
