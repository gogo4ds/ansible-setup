# ansible-setup
Sample setup for ansible for installing basic utils and services

Usage:

1. Make sure to `ssh-copy-id exampl-user@example-server` to your servers from the ansible host.
2. Modify `inventory` by adding your servers and the correct `ansible_ssh_private_key_file` to `[all:vars]`
3. In the root of the repo run `ansible vault create vault.yml` and set your passwords for the servers
4. Run $ `ansible-playbook -i inventory play.yml --ask-vault-pass`
