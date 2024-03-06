# Red-Hat-Satellite-Commands
Included all the commands that I have used so far

# To clean the previous subscriptions
#### subscription-manager unsubscribe --all; 
#### subscription-manager remove --all; 
#### subscription-manager unregister; 
#### subscription-manager clean

# To Register the Clients
#### subscription-manager register --org="ORG-Name" --environment="Library" --force

# Examples to enable repos through CLI
#### subscription-manager repos --enable=rhel-\*-satellite-tools-\*-rpms
#### subscription-manager repos --enable rhel-7-server-extras-rpms
#### subscription-manager repos --enable rhel-7-server-optional-rpms
#### subscription-manager repos --enable rhel-server-rhscl-7-rpms

# List out available subscriptions
#### subscription-manager list --available

# Attach Pool
#### subscription-manager attach --pool=8a7beec875a75ed20179a7683b150b66

# Issues

#### katello-package-upload
#### katello-enabled-repos-upload

# RHEL Satellite Remote Execution
#### useradd rexuser
#### passwd rexuser
#### echo "rexuser   ALL=NOPASSWD:   ALL" | tee -a /etc/sudoers.d/rexuser
