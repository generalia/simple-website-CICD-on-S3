# My Website Deployment

This repository contains a simple website project and a GitHub Actions pipeline for deploying it to an S3 bucket.

## Deployment Workflow

The deployment process is automated using GitHub Actions. Whenever you push updates to the `main` branch, the following steps are performed:

1. GitHub Actions checks out the latest code from the repository.
2. AWS credentials are configured for access to the target S3 bucket.
3. All files, including assets, HTML files, stylesheets, and more, are synchronized with the S3 bucket.

## Usage

To get started:

1. Set up your own AWS S3 bucket.
2. Configure your AWS credentials as GitHub Secrets (`AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY`) in your repository settings.
3. Customize the GitHub Actions workflow (`.github/workflows/deploy.yml`) to match your S3 bucket settings and deployment needs.
4. Push your website files and any updates to the `main` branch.

GitHub Actions will automatically deploy your website to the specified S3 bucket whenever changes are pushed to the `main` branch.

## Image Gallery

The website now includes an image gallery that displays images from the `assets/images/` directory.
