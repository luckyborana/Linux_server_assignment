# Linux Assignment for HeroVired Batch16A - Owned by Lucky Borana

**Repository:** Linux Assignment  
**Environment:** AWS Ubuntu

---

# Project Overview

This project demonstrates the implementation of a **secure, monitored, and automated Linux development environment** for two developers: **Sarah** and **Mike**.

The objective of this assignment is to simulate real-world **DevOps operational practices** including:

- System monitoring
- User management and access control
- Password policy enforcement
- Automated backup configuration
- Backup validation and logging
- Scheduled automation using cron

The environment ensures **system reliability, security, and operational efficiency**.

---
Tasks Detail:

Task 1: System Monitoring Setup

Objective: Configure a monitoring system to ensure the development environment’s health, performance, and capacity planning.

Scenario:

The development server is reporting intermittent performance issues.

New developers need visibility into system resource usage for their tasks.

System metrics must be consistently tracked for effective capacity planning.

Requirements:

Install and configure monitoring tools (htop or nmon) to monitor CPU, memory, and process usage.

Set up disk usage monitoring to track storage availability using df and du.

Implement process monitoring to identify resource-intensive applications.

Create a basic reporting structure (e.g., save outputs to a log file for review).

Task 2: User Management and Access Control

Objective: Set up user accounts and configure secure access controls for the new developers.

Scenario:

Two new developers, Sarah and Mike, require system access.

Each developer needs an isolated working directory to maintain security and confidentiality.

Security policies must ensure proper password management and access restrictions.

Requirements:

Create user accounts for Sarah and Mike with secure passwords.

Set up dedicated directories: 

Sarah: /home/Sarah/workspace

Mike: /home/mike/workspace

Ensure only the respective users can access their directories using appropriate permissions.

Implement a password policy to enforce expiration and complexity (e.g., passwords expire every 30 days).

Task 3: Backup Configuration for Web Servers

Objective: Configure automated backups for Sarah’s Apache server and Mike’s Nginx server to ensure data integrity and recovery.

Scenario:

Sarah is responsible for managing an Apache web server.

Mike is responsible for managing a Nginx web server. 

Both servers require regular backups to a secure location for disaster recovery.

Requirements:

Sarah and Mike need to automate backups for their respective web server configurations and document roots: 

Sarah: Backup the Apache configuration (/etc/httpd/) and document root (/var/www/html/).

Mike: Backup the Nginx configuration (/etc/nginx/) and document root (/usr/share/nginx/html/).

Schedule the backups to run every Tuesday at 12:00 AM using cron jobs.

Save the backups as compressed files in /backups/ with filenames including the server name and date (e.g., apache_backup_YYYY-MM-DD.tar.gz).

Verify the backup integrity after each run by listing the contents of the compressed file.

Expected Output:

Cron job configurations for Sarah and Mike.

Backup files are created in the /backups/ directory.

A verification log showing the backup integrity.

Deliverables

Screenshots or terminal outputs showing successful completion of each task.

A report summarizing the implementation steps and any challenges encountered.

Backup files or verification logs for Task 3.
