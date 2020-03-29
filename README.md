# Ansible-Playbooks
This repo contains useful general purpose Ansible playbooks.
These Playbooks can be used to automate the provisioning of services over remote machines

## How To:
- anpl_hadoop_cluster.yml Playook for whole setup of Hadoop Cluster

    __This PLaybook can be executed as it is__\
    i.e.\
    ansible-playbook anpl_hadoop_cluster.yml
    
- anpl_hadoop_DN.yml	PLaybook for DataNode config in cluster
- anpl_hadoop_NN.yml	PLaybook for NameNode config in cluster
- anpl_hadoop_client.yml	PLaybook for client config in cluster
- anpl_hadoop_jobtracker.yml	PLaybook for Jobtarcker config in cluster
- anpl_hadoop_tasktracker.yml	PLaybook for Tasktarcker config in cluster

    __These Playbooks take IP as the arguements for execution__\
    i.e.\
    ansible-playbook anpl_hadoop_NN.yml -e "ip=127.0.0.1"\
    ansible-playbook anpl_hadoop_DN.yml -e "ip=127.0.0.1"\
    ansible-playbook anpl_hadoop_Client.yml -e "ip=127.0.0.1"\
    ansible-playbook anpl_hadoop_Jobtarcker.yml -e "ip=127.0.0.1"\
    ansible-playbook anpl_hadoop_TaskTracker.yml -e "ip=127.0.0.1"\
    Here 'ip' is the required tag

- anpl_httpd.yml	PLaybook for configuring HTTP Server
- anpl_docker.yml	Playbook for Hadoop cluster config

    __These Playbooks also take IP as the arguements for execution__\
    i.e.\
    ansible-playbook anpl_docker.yml -e "t_ip=127.0.0.1 path=centos:latest"\
    ansible-playbook anpl_httpd.yml -e"t_ip=127.0.0.1"\
    Here the tags used are must
