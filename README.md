# Ansible playbook to mitigate CopyFail and DirtyFrag vulnerabilities
Mitigate CopyFail (CVE-2026-31431) and DirtyFrag (CVE-2026-43284) vulnerabilities in the Linux Kernel using a simple but effective Ansible playbook.
Use this Ansible Playbook to run against your servers or groups. The `target` extra vars option is what you want to use with the host or group entries from your Ansible inventory.

Example: 

```
ansible@ansible:~$ ansible-playbook mitigate-copyfail-dirtyfrag.yaml --extra-vars "target=all_linux"
```

More information in our blog article: [https://www.infiniroot.com/blog/1155/using-nginx-lua-script-mitigate-log4shell-cve-2021-44228-vulnerability](https://www.infiniroot.com/blog/1536/copyfail-cve-2026-31431-mitigation-using-ansible-deployment) .

Contributions and improvements welcome, but lets stick to these two vulnerabilities. This playbook is a quick-fix to share and it is not the plan to make it a "cover all the vulnerabilities" playbook.
