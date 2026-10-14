# Firewall Configuration Guide

## 1. Allow SSH

sudo ufw allow ssh

This command permits SSH connections on port 22 so administrators can access and manage the server remotely.

## 2. Configure Default Policies

sudo ufw default deny incoming
sudo ufw default allow outgoing

The first command blocks incoming connections unless they are explicitly allowed. The second permits outgoing connections from the server.

## 3. Enable the Firewall

sudo ufw enable

This activates UFW and applies the configured firewall policies.

## 4. Allow Web Traffic

sudo ufw allow 8080/tcp

This rule permits TCP connections on port 8080 so users can access the web application.

## 5. Verify Firewall Rules

sudo ufw status verbose
sudo ufw status numbered

These commands display the firewall status, default policies, and numbered rules.

## 6. SSH Safety Note

If UFW is enabled before allowing SSH, remote administrators may lose their connection because incoming SSH traffic could be blocked. Allowing SSH first helps prevent accidental lockout.
