1) The task is to automate the process of installation of webservers and load balancing them using the Automation tool - Ansible

2) First step is to make a secure connection between the host machine and servers. This is done by using SSH-config file.

3) The config file is written in such a way that, if we connect to bastion, we can SSH to all the other hosts in the site local network.

4) The network consists of 5 hosts i.e. HAproxy, devA, devB, devC, Bastion and site-local-network.

5) The HAproxy device will act as an entry point for the service.

6) Then using ansible all three webservers devA, devB ,devC are installed along with HAproxy.

7) Later, the configurations are changed in such a way that the webservers should give us a simple service that displays the hostname, ipaddress of the host.

8) Finally load is balanced equally in round-robin fashion among the webservers using HAproxy. A rudimentary test is added in the end to verify whether the obtained service is correct or wrong. 
