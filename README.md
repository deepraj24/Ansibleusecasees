# Ansibleusecases
# Activities

1. Run preboot tasks, use "yum" for upgrades and use "command" module to "reboot" server

2. Run "wait_for" module to wait for 300 seconds for port 22 to become available before resuming the playbook. the port number can be changed if its not open-ssh
resume playbook on response from port 22

3. Create playbook boilerplate, YAML file. "Change the password for user account, Create and configure a deploy user account, Configure Public Key Authentication for the deploy Account"

4. Add deploy user to sudoers, run updates and upgrades

5. Use "ufw" for iptables configuration, allow only "ssh" traffic, configure "postfix" to relay daily summary email with "debconf" module and customize the ssh_port variable, disable ssh for root account

6. Install ansistrano.rollback using the requirements.yml , add an entry inside it

7. Install the role on the local terminal using ansible-galaxy

8. Create the rollback playbook, add the rollback role inside from the deploy yml file copy parameters required into the rollback file. Now use ansible playbook for rollback mechanism to be applied

9. Write roles using ansible-galaxy, fill in README.md and meta/main.yml, publish, test and tag the role to Git and specify roles and install it in the roles directory

10. All roles that are ready to go to production should be tagged with a version. All playbooks that are ready for production should specify which versions of each role to use
tags and changes to identify version of the playbook to use, store version of playbook with environment




