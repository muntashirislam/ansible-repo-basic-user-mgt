# ansible-repo-basic-user-mgt

This will do basic of these task mentioned bellow. An ansible playbook that I can run against ec2 instances as well as normal linux installations which covers Ubuntu and RedHat servers. It should do the following: 

    - Add new users (the list or the source of these users I leave to your creativity) to these servers and add their ssh key these servers so that after running your playbook, the users should be able to ssh each other without having to use passwords.
 
    - The users should have their own home directory upon logging in.
    - Users should belong to a group that allows them to sudo to root privileges. 
    - The playbook should go through the list of users and compare them against users on the server and get rid of stale users but not important system users.
    - You Ansible playbook should be able to be hooked on to a CI service and it can run i. Syntax check ii. Other tests which you deem necessary (as elaborate as possible, go crazy!) 

=============================Requirement and information before run==================================
1. Add your machine (From where you want to run this play book) ssh key to pub_keys directory.
2. Change your user name on user.yml file
3. Add any user to obsolete_user_list.yml. If the user is stale then playbook will remove it.
4. Change the Inventory file as per requirement.
5. I did not hook this playbook to CI service till now.

This project will update day by day.

