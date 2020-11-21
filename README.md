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
 
 
 ## Automated ELK Stack Deployment

The files in this repository were used to configure the network depicted below.

![TODO: Update the path with the name of your diagram](Images/diagram_filename.png)

These files have been tested and used to generate a live ELK deployment on Azure. They can be used to either recreate the entire deployment pictured above. Alternatively, select portions of the _____ file may be used to install only certain pieces of it, such as Filebeat.

  - _TODO: Enter the playbook file._

This document contains the following details:
- Description of the Topologu
- Access Policies
- ELK Configuration
  - Beats in Use
  - Machines Being Monitored
- How to Use the Ansible Build


### Description of the Topology

The main purpose of this network is to expose a load-balanced and monitored instance of DVWA, the D*mn Vulnerable Web Application.

Load balancing ensures that the application will be highly _____, in addition to restricting _____ to the network.
- _TODO: What aspect of security do load balancers protect? What is the advantage of a jump box?_

Integrating an ELK server allows users to easily monitor the vulnerable VMs for changes to the _____ and system _____.
- : What does Filebeat watch for?_ - **Filebeat** collects data about the file system.
- : What does Metricbeat record?_ - **Metricbeat** collects machine metrics, such as uptime.

The configuration details of each machine may be found below.
_Note: Use the [Markdown Table Generator](http://www.tablesgenerator.com/markdown_tables) to add/remove values from the table_.

| Name     | Function | IP Address     | Operating System |
|----------|----------|------------    |------------------|
| Jump Box | Gateway  | 104.210.72.186 | Linux            |
| Web 1    |          | 10.0.0.5       | Linux            |
| Web 2    |          | 10.0.0.6       | Linux            |
|Elk Server|          | 10.1.0.4       | Linux            |

### Access Policies

The machines on the internal network are not exposed to the public Internet. 

Only the _____ machine can accept connections from the Internet. Access to this machine is only allowed from the following IP addresses:
- _TODO: Add whitelisted IP addresses_

Machines within the network can only be accessed by _____.
- _TODO: Which machine did you allow to access your ELK VM? What was its IP address?_

A summary of the access policies in place can be found in the table below.

| Name     | Publicly Accessible | Allowed IP Addresses |
|----------|---------------------|----------------------|
| Jump Box | Yes/No              | 10.0.0.1 10.0.0.2    |
|          |                     |                      |
|          |                     |                      |

### Elk Configuration

Ansible was used to automate configuration of the ELK machine. No configuration was performed manually, which is advantageous because...
- _TODO: What is the main advantage of automating configuration with Ansible?_

The playbook implements the following tasks:
- _TODO: In 3-5 bullets, explain the steps of the ELK installation play. E.g., install Docker; download image; etc._
- ...
- ...

The following screenshot displays the result of running `docker ps` after successfully configuring the ELK instance.

![TODO: Update the path with the name of your screenshot of docker ps output](Images/docker_ps_output.png)

### Target Machines & Beats
This ELK server is configured to monitor the following machines:
- _TODO: List the IP addresses of the machines you are monitoring_

We have installed the following Beats on these machines:
- _TODO: Specify which Beats you successfully installed_

These Beats allow us to collect the following information from each machine:
- _TODO: In 1-2 sentences, explain what kind of data each beat collects, and provide 1 example of what you expect to see. E.g., `Winlogbeat` collects Windows logs, which we use to track user logon events, etc._

### Using the Playbook
In order to use the playbook, you will need to have an Ansible control node already configured. Assuming you have such a control node provisioned: 

SSH into the control node and follow the steps below:
- Copy the _____ file to _____.
- Update the _____ file to include...
- Run the playbook, and navigate to ____ to check that the installation worked as expected.




