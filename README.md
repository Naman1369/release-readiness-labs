# OrderFlow

This repository contains the Release Readiness Investigation & Deployment Approval Lab.

## Application

A simple Node.js Express application.

### Endpoints
- `GET /`
- `GET /health`

## Current Release
v2.3.0
Production Deployment

## Getting Started

### Clone
```bash
git clone https://github.com/kalvium-devops/release-readiness-lab.git
cd release-readiness-lab
```

### Install
```bash
cd app
npm install
```

### Run
```bash
npm start
```
Alternatively, use Docker Compose:
```bash
docker-compose up --build
```

### Push
Make your changes and push them back to the repository.

## Repository Structure
```
├── .github/
│   └── workflows/
│       └── release.yml
├── app/
│   ├── server.js
│   └── package.json
├── deployment/
│   ├── kubernetes/
│   └── terraform/
├── release/
├── scripts/
├── Dockerfile
├── docker-compose.yml
└── README.md
```

Your team is preparing to release OrderFlow v2.3.0 to production. A deployment pipeline already exists, but multiple production-readiness issues have been intentionally introduced into the repository.

The engineering manager has stopped the release and assigned you as the Release Engineer. Your responsibility is to investigate the repository, identify deployment risks, repair the release pipeline, and prepare the project for a safe production deployment.

The objective is not to deploy the application.Instead, your job is to ensure the repository becomes production-ready.

Repository
Fork and Clone the repository and create a working branch.

git clone https://github.com/kalviumcommunity/release-readiness-labs.git
cd release-readiness-lab

git checkout -b investigation/release-readiness
The repository contains:

a broken GitHub Actions deployment workflow
incomplete release documentation
missing deployment approvals
incorrect version tagging
insecure secret handling
missing rollback strategy
incorrect deployment infrastructure selection
Everything required to complete the assignment already exists inside the repository.

Task 1 — Investigate Release Risks and Repair the Deployment Pipeline
Inspect the deployment workflow and supporting release files.

Identify every issue preventing a safe production deployment.

Repair the deployment workflow so that:

deployment stages execute in the correct order
production deployment requires successful validation stages
release version is correctly referenced
deployment workflow becomes production-safe
After repairing the workflow:

commit your changes
push the branch
verify the workflow executes successfully
Task 2 — Secure the Release Configuration
Inspect the deployment configuration.

Repair every production-readiness issue related to:

secret management
deployment approvals
environment protection
release version traceability
infrastructure selection
The repository intentionally contains incorrect production decisions.

Correct them according to deployment best practices.

Finally, prepare the release so every deployment artifact can be traced back to a unique version.

Task 3 — Prepare the Final Release Readiness Pack
Complete the release preparation by updating the missing operational documentation.

The release package must contain:

release version information
deployment strategy
rollback strategy
deployment infrastructure decision
production approval checklist
deployment validation summary
The completed repository should represent a production-ready release candidate.

Commit the final changes and push them to GitHub.

Required Screenshots
Screenshot 1 — Initial Deployment Investigation
Capture the repository before making any fixes.

The screenshot should clearly show the failed deployment workflow or repository files containing release issues.

Caption (1 line): Describe the production risks discovered before beginning the investigation.

Screenshot 2 — Deployment Pipeline Repairs
Capture the updated deployment workflow after fixing the pipeline stages.

The screenshot should clearly show the corrected workflow configuration inside the editor.

Caption (1 line): Explain how the updated pipeline now supports a safer production deployment.

Screenshot 3 — Secure Release Configuration
Capture the repository after repairing deployment approvals, secret handling, release versioning, and infrastructure configuration.

The screenshot should clearly show the modified configuration files.

Caption (1 line): Explain how the repository now satisfies production deployment requirements.

Screenshot 4 — Successful Validation
Capture the successful GitHub Actions workflow execution after your fixes.

The completed workflow should finish successfully.

Caption (1 line): Explain why the release is now considered deployment-ready.

Screenshot 5 — Final Release Readiness Pack
Capture the completed release documentation together with the final repository state.

The screenshot should clearly show:

release documentation
rollback plan
deployment checklist
release version
Caption (1 line): Summarize why the release can now safely move to production.

Submission
Submit:

One PDF containing all five labelled screenshots
The screenshots must appear in order.

Each screenshot must include its required caption.
