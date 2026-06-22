# AWS CI/CD Automation Portfolio Project

## Project Overview

This project demonstrates the implementation of CI/CD automation using GitHub Actions and AWS services. The project was completed in two phases:

1. AWS Lambda CI/CD Deployment
2. AWS CloudFormation Validation Pipeline

---

## Phase 1: AWS Lambda CI/CD Deployment

### Objective

Build a GitHub Actions workflow that automatically deploys AWS Lambda code whenever changes are pushed to the repository.

### Technologies Used

* AWS Lambda
* Python 3.12
* GitHub Actions
* AWS CLI
* YAML

### Workflow

1. Developer pushes code to GitHub.
2. GitHub Actions workflow is triggered.
3. Dependencies are installed.
4. AWS credentials are configured.
5. Lambda package is created.
6. Lambda function is updated automatically.

### Key Skills Demonstrated

* Serverless Computing
* CI/CD Automation
* GitHub Actions
* AWS Lambda Deployment
* Python Development

### Challenges Encountered

* Workflow file placement issues
* YAML syntax errors
* Python installation and configuration
* GitHub Actions trigger configuration

### Outcome

✅ Successfully automated Lambda deployment using GitHub Actions.

---

## Phase 2: AWS CloudFormation Validation Pipeline

### Objective

Implement a GitHub Actions workflow to automatically validate CloudFormation templates before deployment.

### Technologies Used

* AWS CloudFormation
* GitHub Actions
* AWS CLI
* YAML

### Workflow

1. CloudFormation template is committed to GitHub.
2. GitHub Actions workflow is triggered.
3. AWS credentials are configured.
4. CloudFormation template is validated automatically.
5. Validation results are displayed in GitHub Actions.

### Key Skills Demonstrated

* Infrastructure as Code (IaC)
* CloudFormation Template Development
* Automated Validation
* CI/CD Pipeline Troubleshooting

### Challenges Encountered

* Incorrect workflow locations
* Missing workflow triggers
* CloudFormation validation failures
* Invalid template characters
* Repository structure issues

### Outcome

✅ Successfully validated CloudFormation templates through GitHub Actions.

---

## Repository Structure

```text
lambda-cicd
│
├── README.md
│
├── cloudformation
│   └── s3-bucket.yml
│
├── lambda
│   ├── lambda_function.py
│   └── requirements.txt
│
└── .github
    └── workflows
        ├── lambda.yml
        └── cfn-validate-pr.yml
```

## Overall Results

✅ Automated AWS Lambda deployments

✅ Automated CloudFormation validation

✅ Integrated GitHub Actions with AWS

✅ Gained hands-on experience with CI/CD, Serverless Computing, and Infrastructure as Code

## Lessons Learned

This project reinforced the importance of:

* CI/CD automation
* Infrastructure as Code
* Cloud security best practices
* GitHub Actions troubleshooting
* AWS service integration
* Systematic problem solving

```
```
## Screenshots

### GitHub Actions Success
[Insert Screenshot]

### AWS Lambda Function
[Insert Screenshot]

### CloudFormation Validation Workflow
[Insert Screenshot]

### Repository Structure
[Insert Screenshot]