## Deploy a high-availability web app using CloudFormation

### Scenario
Your company is creating an Instagram clone called Udagram, and the requirement is to deploy this new application to the AWS infrastructure using Infrastructure as Code.

You have been tasked with provisioning the required infrastructure and deploying a dummy application, along with the necessary supporting software.

Since the underlying network infrastructure will be maintained by a separate team, you must create independent stacks for the network infrastructure and the application itself.

Infrastructure spin up and tear down needs to be automated so that each team can create and discard testing environments on demand.


To access the web app hosted click [here](http://projec-webap-eh8l8x1txque-296288662.us-east-2.elb.amazonaws.com/) 

### Creating the Network Stack
```
create.sh project-2-network networks.yml network-parameters.json
```

### Updating the Network Stack
```
update.sh project-2-network networks.yml network-parameters.json
```

### Creating the Server Stack
```
create.sh project-2-udagram udagram.yml udagram-parameters.json
```


### Updating the Server Stack
```
update.sh project-2-udagram udagram.yml udagram-parameters.json
```