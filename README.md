Testing
=====================

Remember to change the all.yaml file and add your ssh-rsa key and your username, etc
ADD all the hosts under inventory.ini that you need to ssh

Trigger like this: ansible-playbook -vvv -i inventory.ini test-lambodar.yaml -e hostname=testing_host

"testing_host" can be modified to any host 

The name of the file that I am changing is testing_larry

The format of the file is as follow:
[host_name]
  host=[testing]

However, if the format is different you will need to modify the regex 

Alternative, you can just use a cmd action 
