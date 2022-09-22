First:
  We need to install ansible in our machines
  know where is our private ssh key
  setting up the address in our inventory file
  and make a ping with the command:
  the command to run on my local = ansible -m ping omnia -i ~/learn/omnia/omnia-nodes-test/ansible/config/hosts

  after a successfull ping, we need to apply a playbook to update and install docker and docker compose with the command: ansible-playbook ansible/playbooks/docker.yml -l digitalocean -i ~/learn/omnia/omnia-nodes-test/ansible/config/hosts

  after that we can apply each node running the command specified into the Readme file in each chain folder 
