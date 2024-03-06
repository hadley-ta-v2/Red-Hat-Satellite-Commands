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

subscription-manager list --available





sudo subscription-manager list --available

subscription-manager attach --pool=8a7beec875a75ed20179a7683b150b66


subscription-manager repos --enable 


subscription-manager repos --enable=rhel-\*-satellite-tools-\*-rpms
yum -y install katello-agent

RHEL9


 47  subscription-manager register --org="ADEK" --environment="Library"
   48  yum repolist
   49  yum install telnet
   50  subscription-manager --list
   51  subscription-manager auto-attach
   52  subscription-manager list
   53  subscription-manager --enable=*rhel9*
   54  subscription-manager repo --enable=*rhel-9*
   55  subscription-manager repos --enable=*rhel-9*
   56  yum repolist
   57  yum install telnet
   58  df -




### Issues

katello-package-upload
katello-enabled-repos-upload

useradd rexuser
passwd rexuser
echo "rexuser   ALL=NOPASSWD:   ALL" | tee -a /etc/sudoers.d/rexuser
