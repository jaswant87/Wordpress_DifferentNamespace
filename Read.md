Ansible code is tested over lab cluster hence code pushed from remote host to kuberentes API server (i.e master)
Ansible code can be pushed remotely withcopying kubernetes manifests file that will need copy of kubeconfig to admin/remote system
For persistent volume Hostpath  volume is used hence single replica is used.
For HA using more replicas dynamic Storage Class (NFS) can be used.
As most environment use Resource ruoata and pod policies, resource limits are not used but if needed can be used.


Usage:- ansible-playbook Playbook_Wordpress.yml