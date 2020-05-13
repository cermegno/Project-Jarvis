# Project-Jarvis
Automated provisioning of end-to-end application stack on PowerOne with Ansible
## Description
In this project I try to automate the provisioning of an application stack on top of DellEMC PowerOne through Ansible. Jarvis takes some high level or even business level questions about the application stack required, ex: number of users for a LAMP stack, etc. It starts by creating a new ESX cluster for the desired application stack. Then creates the VMs that are required to support an environment of the specified size and then installs and configures the applications in each of the VMs

The inspiration for Jarvis project name comes from the Aritificial Intelligence Tony Stark uses in Avengers movies. Like in the movies, the aspiration is to actually interact with Jarvis via voice
## About PowerOne
DellEMC PowerOne is a converged infratructure solution that includes compute, networking and storage elements on a single system. PowerOne simplifies the management of the underlying components through a single API which for example allows teams to provision an ESX cluster with a single API call. Jarvis uses the URI Ansible module to interact with the PowerOne API
## Artifacts
- PowerOne Postman. It shows how to perform CRUD operations for Cluster Resource Groups (think ESX clusters) in addtion to some basic GET operations that provide information abou the system itself. You can test it against the PowerOne simulator if you have access to it, or against a real PowerOne system. Physical PowerOne systems require logging in and getting a bearer token. If you are using this Postman collection against a real system, first create an environment in Postman with a single variable called "token". Finally, the collection includes sample responses for every API call
- Playbooks and Python scripts to follow soon
- Excel calculator for LAMP stack sizing to follow soon
