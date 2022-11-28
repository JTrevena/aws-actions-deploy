Default "create-react-app" app is currently hosted on amplify on a pull-based system. The goal of this project is to migrate the app to be hosted on a new AWS service (likely an EC2 instance) using terraform and github CI.

Currently, pushing changes to main triggers a workflow which runs and applies the terraform in ```main.tf```. This workflow creates a new VPC in AWS.
