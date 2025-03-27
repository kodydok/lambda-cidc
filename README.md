# lambda-cidc

Created an end-to-end cicd pipeline for our lambda serverless application

Pull request event - CICD for CloudFormation test stacks

Validate-cfn:
-config aws credentials
-validate cloudformation template
-deploy stack
-comment on pull request

Cleanup-on-merge:
- config aws credentials
- deletes test stack IF github pull request was merged
