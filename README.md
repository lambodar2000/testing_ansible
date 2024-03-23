Testing
=====================

1. Remember to change the all.yaml file and add your ssh-rsa key and your username, etc
2. ADD all the hosts under inventory.ini that you need to ssh
3. pip install ansible

4. Trigger like this: ansible-playbook -vvv -i inventory.ini test-lambodar.yaml -e hostname=testing_host -e path_file=/root/testing_larry ("testing_host" can be modified to any host, and path_file is the path to your existing file) 

5. The name of the file that I am changing is testing_larry ( For your convinience I am putting the file in this repo as well :) ) 
The format of the file is as follow:
[host_name]
  host=[testing]

However, if the format is different you will need to modify the regex 

5. Alternative, you can just use a cmd action 
