#  Infrastructure as Code using CloudFormation
This folder provides the ClooudFormation template to deploy as web server in two availability zones.  

## Dependencies
### 1. AWS account
You would require to have an AWS account to be able to build cloud infrastructure.

### 2. VS code editor
An editor would be helpful to visualize the image as well as code. Download the VS Code editor [here](https://code.visualstudio.com/download).

## Architecture

Below is the project architecture

![architecture](architecture.jpeg)

## How to run the scripts.
```bash
# Ensure that the AWS CLI is configured before runniing the command below
# Create the network infrastructure
# Check the region in the create.sh file
./create.sh infraStack network.yml network-parameters.json
# Create servers
# Change the AMI ID and key-pair name in the servers.yml
# Check the region in the update.sh file
./update.sh serverStack servers.yml server-parameters.json
```
