# Prometheus and Grafana Lab

## Contents

This lab contains a Kubernetes manifests to deploy Prometheus and Grafana into the OpenShift lab environment.

It also contains Python Flask backend that has been instrumented with a `/metrics` endpoint to be consumed by Prometheus.

## Credits

[John J. Rofrano](https://www.coursera.org/instructor/johnrofrano) Senior Technical Staff Member, DevOps Champion, @ IBM Research  

## Git workflow

1. Check the current Remote
`git remote -v` 

2. Change the Remote URL 
`set remote set-url origin https://github.com/thoimai/monitoring-systems.git` 

3. Create access token to authorize access to github acc from my local machine  
`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`

4. Switch to the *main* branch 
`git branch -M main` 

5. Push to my remote repo hosted on github

`git push -u origin main` 

---
# LAB SETUP 

## Infrastructure assessment 

* How to know how many computing resources (vRAM, RAM, storage) my server machine has: 

As a system administrator, when you're given a server, you'll want to assess various parameters and attributes to understand its capabilities and suitability for running software. Here's a breakdown of what you might look at and how you can find this information:

### 1. **Hardware Specifications**:
   - **Processor (CPU)**: Type, cores, threads, and clock speed.
   - **Memory (RAM)**: Total size and speed.
   - **Storage**: Type (HDD, SSD), capacity, and speed.
   - **Network Interface Cards (NICs)**: Speed and configuration.
   - **Graphics Processing Unit (GPU)** if applicable.

   **How to Find**: Use commands like `lscpu`, `free -m`, `lsblk`, `lspci`, `ifconfig`, or `ip a`.

### 2. **Operating System and Software**:
   - **OS Version**: Compatibility with the software you plan to run.
   - **Installed Software**: Existing applications and services.
   - **Available Updates**: Security and feature updates.

   **How to Find**: Use commands like `uname -a`, `lsb_release -a`, `dpkg --list`, `rpm -qa`.

### 3. **Performance Metrics**:
   - **CPU Utilization**: How much of the CPU is being used.
   - **Memory Usage**: Amount of RAM in use.
   - **Disk I/O**: Read/write speeds.
   - **Network Utilization**: Bandwidth usage.

   **How to Find**: Tools like `top`, `htop`, `iostat`, `vmstat`, `iftop`.

### 4. **Security Configuration**:
   - **Firewall Settings**: Open and closed ports.
   - **User Accounts**: Existing users and permissions.
   - **Security Policies**: Compliance with organizational standards.

   **How to Find**: Use commands like `iptables -L`, `ufw status`, `cat /etc/passwd`.

### 5. **Virtualization and Containerization Support**:
   - **Hypervisor**: Type and version if virtualization is used.
   - **Containerization**: Tools like Docker if containerization is required.

   **How to Find**: Commands like `virt-what`, `docker info`.

### 6. **Scalability and Redundancy**:
   - **Clustering Capabilities**: For high availability.
   - **Backup Solutions**: Existing backup strategies.

### 7. **Compliance and Licensing**:
   - **Software Licenses**: Ensure all software is properly licensed.
   - **Compliance Standards**: Adherence to legal and organizational policies.

By evaluating these aspects, you can gain a comprehensive understanding of the server's capabilities and limitations. This information will guide you in setting up additional software and configuring the server to meet the requirements of your next project.