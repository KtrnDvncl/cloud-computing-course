<div align="center">

# CCM101 - Cloud Computing
## Enterprise Cloud Architect - Operational Manual

**Project:** Secure Multi-Tier Web Application
**Application Stack:** WordPress + MySQL
**Prepared by:** James Russel Lopez | Vicel Mae Peralta | Mark Lester Dela Cruz | Katrina Advincula
**Section:** BSIT 4H
**Instructor:** Jenkielyn C. Torres
**Date:** October 2026

</div>

---

## 1. Deployment Guide

This manual provides the IT team with the necessary steps to deploy the application infrastructure on the Ubuntu Server VM. 

To deploy the multi-tier containerized application, navigate to the directory containing the `docker-compose.yml` file and execute the following command:

```bash
docker compose up -d
```

*Note: The `-d` flag runs the containers in "detached" mode, allowing them to run in the background so you can continue using the server terminal.*

## 2. Maintenance and Disaster Recovery

A custom Bash shell script (`automation-script.sh`) has been implemented to manage system backups autonomously. This script is scheduled via a Cron Job.

* **Backup Storage Location:** The automated database backups are safely stored on the Ubuntu Server in the `/var/backups/app-data/` directory. 
* **Data Persistence:** Because we utilized persistent volumes in our Docker configuration, all data will survive a VM reboot or container failure.
