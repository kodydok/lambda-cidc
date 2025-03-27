# lambda-cidc

Push event - cicd pipeline for our lambda serverless application

deploy-lambda:
- sets up python environment
- installs any packages
- configure aws credentials
- zips lambda directory and updates lambda function

Pull request event - CICD for CloudFormation test stacks

validate-cfn:
- configure aws credentials
- validate cloudformation template
- deploy stack
- comment on pull request

cleanup-on-merge:
- configure aws credentials
- deletes test stack IF github pull request was merged
