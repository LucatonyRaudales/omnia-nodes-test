# Omnia - Tony Raudales test

challenge: Run differents blockchains nodes for mainnet and testnet.

## How to run the nodes?
I used docker/docker-compose to run the nodes, each chain have a specific folder that contain the docker-compose manifest.

I used ansible tool to provision and manage the nodes in whatever vm, you only need to configure a new vm on ./ansible/config/host file.

To use [ansible](https://www.ansible.com/) you need install it.

steps to use this repository: 

- We need to install ansible in our machines.
  
- know where is our private ssh key

- setting up the address in our inventory file(./ansible/config/hosts)

- and make a ping with the command at the root of this repository:
```bash
ansible -m ping omnia -i ~/learn/omnia/omnia-nodes-test/ansible/config/hostsr
```
the output should be success.
 
After that we can apply each node running the command specified into the Readme file in each chain folder 
## See you soon Omnia!