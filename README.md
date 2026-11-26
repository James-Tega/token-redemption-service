# Token Redemption Service



## Architecture
API Gateway (HTTP API) → Lambda (Python 3.12) → DynamoDB.
Infrastructure in Terraform; CI/CD with GitHub Actions using OIDC (no stored AWS keys).

## Status
In progress. Currently on Issue #1 (repo setup).

## Local setup
    py -m pip install pre-commit
    py -m pre_commit install
