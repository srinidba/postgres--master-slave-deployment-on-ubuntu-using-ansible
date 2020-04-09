-- Update the inventory hosts file with the required values 
db_hosts - specify all the hosts
master_hosts - specify only the master host
slave_hosts - specify the slave hosts

-- Run the main ansible playbook as below with verbose option
 ansible-playbook -i hosts postgres_setup.yaml -vv
 
Additional information:
--below are playbooks and files available on the directory
postgres_setup.yaml 		---->    Main playbook setup file which calls all the modules
pg_install.yaml				---->	 Postgres installation playbook
pg_master_setup.yaml		---->	 Postgres master setup playbook
pg_slave_setup.yaml			---->    Postgres slave setup playbook
hosts						---->    Inventory file
