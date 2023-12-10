CI/CD Demonstration of group project
Related group project : PlaceholderOrganization/memorize-frontend

Resource Links
Backend

Repository
Deployed-Webapp-main
Deployed-Webapp-staging
Deployed-Webapp-dev
Frontend

Repository
Live-site: www.danviktor.dk
Pre-prod : staging-test.danviktor.dk
Development: dev-test.danviktor.dk
Database
Created as a MySQL database running in a docker container a Linux VM on Azure

Branching Strategy
We use the 'main' branch as our released codebase. For new developments, we create feature branches from our development branch. Once a feature is complete, we initiate a pull request to merge it into the 'development' branch. This triggers automated builds and tests via GitHub Actions, and if successful, the changes are deployed to Azure Dev Web App service. When the sprint is complete, we deploy our successfully deployed development branch to our staging branch for further testing. When customer accepts the changes, we merge staging into main.

Key elements in strategy

Main Branch (live production)
Staging Branch (pre-production)
Development Branch (continous development)
Feature Branches
Pull Requests (Approval required from another team member)
Continuous Integration (CI) with GitHub Actions
Deployment with Azure Web App Service
Merging Staging into Master
