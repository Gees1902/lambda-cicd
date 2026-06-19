# lambda-cicd
Lambda Continuous Integration Continuous  Delivery  Continuous Deployment

# AWS Lambda CI/CD Pipeline with GitHub Actions

## Project Overview

This project demonstrates how to automate AWS Lambda deployments using GitHub Actions and AWS CLI. The goal is to eliminate manual deployments and implement a secure, repeatable CI/CD process that automatically updates a Lambda function whenever code changes are pushed to GitHub.

This project helped me gain hands-on experience with serverless computing, GitHub Actions workflows, AWS IAM permissions, and secure deployment automation.

---

## Project Objectives

* Create an AWS Lambda function using Python.
* Store Lambda source code in GitHub.
* Build a GitHub Actions workflow for automated deployments.
* Configure secure AWS authentication using GitHub Secrets.
* Automatically package and deploy Lambda code after commits are pushed to the repository.
* Gain practical experience with CI/CD and DevSecOps concepts.

---

## Technologies Used

* AWS Lambda
* GitHub
* GitHub Actions
* AWS CLI
* Python
* IAM
* YAML

---

## Project Structure

```text
lambda-cicd/
│
├── lambda/
│   ├── lambda_function.py
│   ├── requirements.txt
│   └── .github/
│       └── workflows/
│           └── lambda-deploy.yaml
```

---

## CI/CD Workflow

1. updates Lambda code.
2. Code is committed and pushed to GitHub.
3. GitHub Actions automatically triggers the workflow.
4. Dependencies are installed.
5. AWS credentials are securely loaded from GitHub Secrets.
6. Lambda package is created.
7. AWS Lambda function is updated automatically.
8. Deployment completes without manual intervention.

---

## GitHub Actions Workflow

The workflow is configured to:

* Trigger on pushes to the main branch.
* Install Python dependencies.
* Configure AWS credentials securely.
* Package Lambda code into a deployment archive.
* Deploy updated code to AWS Lambda.

This automation reduces deployment errors and ensures consistency across deployments.

---

## Security Considerations

### Secrets Management

AWS credentials are stored in GitHub Secrets instead of hardcoded in source code.

Examples:

* AWS_ACCESS_KEY_ID
* AWS_SECRET_ACCESS_KEY

This helps prevent accidental exposure of sensitive credentials.

### Least Privilege

IAM permissions should be restricted to only the actions required for Lambda deployments.

Examples:

* lambda:UpdateFunctionCode
* lambda:GetFunction
* logs:CreateLogGroup
* logs:CreateLogStream
* logs:PutLogEvents

### Version Control

All changes are tracked through Git, providing:

* Change history
* Auditability
* Rollback capability
* Collaboration support

---

## Benefits of CI/CD for Cloud Security

Implementing CI/CD provides several security and operational advantages:

* Reduces manual deployment errors.
* Improves consistency across environments.
* Enables rapid deployment of security fixes.
* Creates an auditable deployment process.
* Supports Infrastructure as Code and DevSecOps practices.
* Increases deployment reliability.

---

## Challenges Encountered

During this project I encountered several common issues:

* PowerShell does not support the Linux `touch` command.
* Python installation and PATH configuration.
* YAML formatting and indentation requirements.
* GitHub Actions workflow troubleshooting.
* AWS credential configuration.
* Lambda deployment packaging.

Resolving these issues provided valuable real-world troubleshooting experience.

---

## Lessons Learned

This project strengthened my understanding of:

* AWS Lambda
* Serverless architecture
* Git and GitHub workflows
* GitHub Actions
* CI/CD pipelines
* IAM security best practices
* Automated cloud deployments
* DevSecOps principles

---

## Future Enhancements

Future improvements may include:

* Infrastructure as Code using Terraform or CloudFormation.
* Automated security scanning.
* Unit testing integration.
* Multi-environment deployments (Dev, Test, Production).
* AWS CodePipeline integration.
* CloudWatch monitoring and alerting.

---

## Conclusion

This project demonstrates how modern cloud teams can automate serverless deployments using GitHub Actions and AWS Lambda. By combining version control, automation, and security best practices, organizations can deploy applications faster, more consistently, and with reduced operational risk.
