# hng13-stage1-devops
Automated Deployment Bash Script

# What the repo contains
deploy.sh : Main automated deployment script
README.md : This file
test.html: test code 

# Prerequisites
Local: git, bash, ssh, rsync, curl
Remote: Linux VM, SSH key access
Cloud: GCP with firewall allowing SSH & HTTP (port 22 & 80)

# How to run
1. Script is executable:
   chmod +x deploy.sh

2. Run:
   ./deploy.sh
   Follow prompts: Git URL, PAT, branch, remote user & host, SSH key path, app port.

3. For cleanup:
   ./deploy.sh --cleanup

# Notes
Script logs to ./deploy_YYYYMMDD_HHMMSS.log
Was tested on a disposable VM before production
