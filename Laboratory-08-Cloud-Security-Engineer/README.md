# Laboratory 08: The Cloud Security Engineer

## Mission Overview

This laboratory focuses on securing an Ubuntu server using UFW (Uncomplicated Firewall). The activity involves deploying a web application, reviewing network access, and configuring firewall rules to allow legitimate traffic while blocking unauthorized incoming connections.

## Objectives

- Understand the Principle of Least Privilege and attack surface.
- Review the importance of securing network ports.
- Configure UFW with a Default Deny incoming policy.
- Allow SSH and web application traffic.
- Document firewall configurations and security practices.

## Commands Executed

docker run -d --name secure-web-app -p 8080:80 nginx
curl http://localhost:8080
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
sudo ufw allow 8080/tcp
sudo ufw status numbered

## Skills Learned

I learned how to deploy a web application, configure firewall rules, control network access, and verify active security policies. I also learned why unnecessary open ports should be restricted to reduce security risks.

## Screenshots

- `screenshots/vulnerable-app-running.png`
- `screenshots/firewall-activated.png`
- `screenshots/firewall-port-allowed.png`
