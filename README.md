# k8s
An initial working set of Ansible scripts to deploy kubernetes to a cluster.

ansible-playbook -Kki hosts --ask-vault-pass 0_initial.yml

ansible-playbook -Kki hosts --ask-vault-pass 02_kubernetes-dependencies.yaml

ansible-playbook -Kki hosts --ask-vault-pass 02.1_dependencies.yaml

ansible-playbook -Kki hosts --ask-vault-pass 03_master.yaml

ansible-playbook -Kki hosts --ask-vault-pass 04_join_podnet.yaml


# References:
https://www.arubacloud.com/tutorial/how-to-create-kubernetes-cluster-with-kubeadm-and-ansible-ubuntu-20-04.aspx

https://www.linuxsysadmins.com/install-kubernetes-cluster-with-ansible/
