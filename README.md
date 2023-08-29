# ansible-rhel9-oscap-hipaa
Some playbooks to automate the scanning, patching, reporting and remediation of RHEL

## Run the setup of OpenScap and its dependencies for RHEL 9
ansible-playbook ./setup_oscap.yml -i inventory

## Run a scap report / audit
ansible-playbook ./run_scap_report.yml -i inventory 

## Configure a webserver and deploy the reports
ansible-playbook ./deploy_scap_report.yml -i inventory

## Patch the server 
ansible-playbook ./patch_os.yml -i inventory 