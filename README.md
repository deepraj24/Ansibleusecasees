# Ansibleusec
Activities
run preboot tasks, use "yum" for upgrades
use "command" module to "reboot" server
run "wait_for" module to wait for 300 seconds for port 22 to become available before resuming the playbook. the port number can be changed if its not open-ssh
resume playbook on response from port 22

Create playbook boilerplate, YAML file
"Change the password for user account, Create and configure a deploy user account,
Configure Public Key Authentication for the deploy Account"
Add deploy user to sudoers, run updates and upgrades
use "ufw" for iptables configuration, allow only "ssh" traffic
configure "postfix" to relay daily summary email with "debconf" module
customize the ssh_port variable, disable ssh for root account

Install ansistrano.rollback using the requirements.yml , add an entry inside it
install the role on the local terminal using ansible-galaxy
create the rollback playbook, add the rollback role inside
from the deploy yml file copy parameters required into the rollback file
now use ansible playbook for rollback mechanism to be applied

Write roles using ansible-galaxy, fill in README.md and meta/main.yml
publish, test and tag the tole to Git
specify roles and install it in the roles directory
All roles that are ready to go to production should be tagged with a version. All playbooks that are ready for production should specify which versions of each role to use
tags and changes to identify version of the playbook to use, store version of playbook with environment




