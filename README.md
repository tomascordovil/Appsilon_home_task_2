## Configuration Management Task 

Start by installing Docker in your linux machine

Continue by installing ansible:
    sudo apt install ansible

The install molecule:
    pip install molecule

Select docker as the driver to use:
    molecule init role --role-name ansible-role-nginx --driver-name docker

Change directory to be in the same directory as the playbook.
Make sure Docker is running on your local machine.

Run the following command to create a container:
    molecule create

Execute the playbook on the container:
molecule converge

After the playbook has been executed successfully you can now delete/remove the container:ove the container:
    molecule destroy