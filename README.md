## Configuration Management Task 

Start by installing Docker in your linux machine (see https://www.docker.com/products/docker-desktop/)

Continue by installing ansible:
    sudo apt install ansible

Then, install molecule:
    pip install molecule

Select docker as the driver to use:
    molecule init role --role-name ansible-role-nginx --driver-name docker

Change directory to be in the same directory as the playbook.
Make sure Docker is active and running on your local machine.

Run the following command on a terminal to create a container:
    molecule create

Execute the playbook on the container by executing this command on a terminal:
    molecule converge

After the playbook has been executed, you can now exit and destroy the container:
    molecule destroy
