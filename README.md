name: Inemesit Dominic
slack name: Dominic.A
project description: Automated Web Deployment with GitHub Actions and NGINX
Project Overview
This DevOps project demonstrates how to automate the deployment of a custom webpage using GitHub Actions and NGINX.
It showcases key DevOps principles including CI/CD, infrastructure-as-code, and automated provisioning of a live web server.
 Technologies Used
- GitHub Actions – for CI/CD automation
- NGINX – as the web server
- Ubuntu Server – hosting environment (can be cloud-based or local VM)
- HTML – for the custom webpage

 Setup Instructions
1. Clone the Repository
git clone https://github.com/IndomakHub/hng13-stage0-devops-Project.git
cd your-repo-name
2. Configure NGINX
Update nginx/default.conf with your desired server settings. This file will be used to configure NGINX during deployment.
3. Customize Your Webpage
Edit src/index.html to reflect your custom content.
4. Set Up GitHub Secrets
Add the following secrets to your GitHub repository:
- SERVER_IP – IP address of your NGINX server
- SSH_USER – SSH username
- SSH_KEY – Private SSH key for authentication
5. GitHub Actions Workflow
The deploy.yml workflow:
- Triggers on push to main
- Connects to the server via SSH
- Copies updated files
- Reloads NGINX to serve the latest content
   Accessing the Webpage
Once deployed, your webpage will be accessible at http://<SERVER_IP>.

