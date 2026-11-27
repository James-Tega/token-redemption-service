# Token Redemption Service

This service creates single-use tokens, such as OTPs, with an expiry period.
If two requests try to redeem the same token at the same time, only one succeeds and the other is rejected as already used.
## Architecture
API Gateway (HTTP API) → Lambda (Python 3.12) → DynamoDB.
Infrastructure in Terraform; CI/CD with GitHub Actions using OIDC (no stored AWS keys).

## Status
In progress. Currently on Issue #1 (repo setup).

## Local setup
    py -m pip install pre-commit
    py -m pre_commit install
    py -m pre_commit run --all-files
