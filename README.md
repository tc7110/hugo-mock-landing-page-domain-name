# hugo-mock-landing-page-domain-name

Author: Tiana Costello

This repository hosts the auto-deployed version of the Hugo landing page developed for CIS 3500's Spring 2024 Homework 2, Part II. It builds on the initial project from Homework 1, where we customized a landing page using the hugo-bootstrap-theme to showcase a chosen product's features based on user stories.

The published site can be accessed at https://tc7110.github.io/hugo-mock-landing-page-domain-name/.

# 🚀 Deployment

The project has been advanced by importing the work from Homework 1 into this repository and updating the baseURL in the config.toml. Necessary repository settings adjustments were made to facilitate automated deployment through GitHub Actions.

The deployment process is automated with a GitHub Actions workflow defined in .github/workflows/gh-pages-deployment.yaml. This workflow:

Activates on pushes to the main branch.
Runs on an Ubuntu 22.04 environment.
Checks out the repo, including submodules for Hugo themes.
Sets up Hugo, compiles static files with minification and drafts included, and deploys to the gh-pages branch.
Integrates a custom domain, ecospend.click, by uncommenting and setting the cname in the workflow file.
A detailed explanation of each step is provided in the workflow file comments, guiding through setup, build, and deployment phases.

After configuring and verifying GitHub Actions, the site was successfully deployed and further validated by updating a link to encourage user issues, demonstrating the efficacy of the CI/CD pipeline.


