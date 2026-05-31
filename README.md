# Multi-Tenant Odoo Deployment with Nginx Reverse Proxy

## Overview

This project demonstrates the deployment of three independent Odoo environments, each with its own PostgreSQL database, behind a centralized Nginx reverse proxy.

The architecture provides a multi-tenant setup where multiple companies can operate separate Odoo instances while sharing the same infrastructure. Nginx handles request routing, SSL termination, and domain-based access to each Odoo deployment.

---

## Architecture

Users access company-specific domains through Nginx, which forwards requests to the appropriate Odoo instance.

Example:

company1.example.com → Odoo Instance 1 → PostgreSQL Database 1

company2.example.com → Odoo Instance 2 → PostgreSQL Database 2

company3.example.com → Odoo Instance 3 → PostgreSQL Database 3

---

## Features

* Three isolated Odoo deployments
* Dedicated PostgreSQL database per company
* Nginx reverse proxy for request routing
* Domain-based access to each company
* SSL/TLS support
* Centralized web access management
* Scalable multi-tenant architecture
* Simplified administration and maintenance

---

## Components

### Odoo

* Company 1 Odoo Instance
* Company 2 Odoo Instance
* Company 3 Odoo Instance

### Database

* PostgreSQL Database 1
* PostgreSQL Database 2
* PostgreSQL Database 3

### Reverse Proxy

* Nginx
* SSL termination
* Domain routing
* Load distribution

---

## Benefits

* Separation of company data
* Independent database management
* Reduced infrastructure costs
* Easier maintenance and upgrades
* Improved security through tenant isolation
* Centralized access through Nginx

---

## Deployment Workflow

1. Deploy PostgreSQL databases.
2. Deploy Odoo instances.
3. Configure Nginx reverse proxy.
4. Configure DNS records.
5. Enable SSL certificates.
6. Verify access to each company domain.

---

## Example Access URLs

* https://company1.example.com
* https://company2.example.com
* https://company3.example.com

---

## Technologies Used

* Odoo
* PostgreSQL
* Nginx
* Linux
* Docker (Optional)
* SSL/TLS

---

## Author

Mostafa Magdy

DevOps | Cloud | Linux | Infrastructure Automation
