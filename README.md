# How to use Ansible Roles

This is an example Ansible project, demonstrating how to write and reuse ansible Roles.
Inside `roles` folder there are two roles named `packageRemover` and `apacheInstaller`. There are called inside `test-role.yaml` file.
- `packageRemover` is first used to remove any previous installation of `apache`. You can reuse it to remove any other package. To do so, inside `vars` file change the value of `package` var.
- `apacheInstaller` is then used to install a fresh `apache`. 
## Requirement

Requirement         | Specification
------------------- | ----------------------
OS                  | Ubuntu 22.04
Language            | Ansible


## How to use

Install `ansible`, clone this project, and then Simply run:

```bash
ansible-playbook test-role.yaml
```
- To determine the address of your target server for configuration refer to `hosts` file. 
