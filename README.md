# ansible-f5-prep
A quick playboopk for installing the needed python modules and repositories for using Ansible for F5 automation

## Configuration
If this is being run in an environment with a Red Hat Satellite server, Pulp server, or some local EPEL host, update the variables {{ epel_repo_url }} and {{ epel_repo_url_gpg_key }} to match your local environment

## Usage
On your ansible (or ansible tower) nodes, run either playbook directly from the command line

`ansibe-playbook playbook.yml` (if the EPEL repositories can be enabled in your environment)
or
`ansible-playbook no-epel.yml` (if EPEL is not allowed or available in your environment)
