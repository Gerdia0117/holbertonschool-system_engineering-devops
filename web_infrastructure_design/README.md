# Web Infrastructure Design

This project focuses on designing and understanding various web infrastructure architectures. Each task involves creating diagrams and explaining the components, their roles, and potential issues in different web infrastructure setups.

## Project Overview

The goal of this project is to develop a deep understanding of web infrastructure by designing systems from simple to complex, covering aspects such as:
- Server architecture
- Load balancing
- Database management
- Security
- Monitoring
- Scalability and redundancy

## Learning Objectives

By the end of this project, you should be able to explain:
- What a server is and where servers are located
- What DNS is and its role in web infrastructure
- What a web server is and its purpose
- What an application server is and how it differs from a web server
- What a database is and its role in the infrastructure
- How client-server communication works
- Different types of DNS records (A, CNAME, TXT, MX)
- The concepts of single points of failure (SPOF)
- How to avoid downtime during deployments
- The importance of high availability and scalability
- Load balancing algorithms and configurations
- Active-Active vs Active-Passive setups
- Primary-Replica database clusters
- Security considerations (firewalls, HTTPS, monitoring)

## Tasks

### 0. Simple Web Stack

**File:** `0-simple_web_stack`

Design a basic one-server web infrastructure that hosts a website reachable via `www.foobar.com`.

#### Requirements:
- 1 server
- 1 web server (Nginx)
- 1 application server
- 1 application files (your code base)
- 1 database (MySQL)
- Domain name `foobar.com` configured with a `www` record pointing to server IP `8.8.8.8`

#### You must explain:
- What is a server
- The role of the domain name
- What type of DNS record `www` is in `www.foobar.com`
- The role of the web server
- The role of the application server
- The role of the database
- How the server communicates with the user's computer

#### Issues with this infrastructure:
- **SPOF (Single Point of Failure):** The entire website relies on a single server
- **Downtime during maintenance:** When deploying new code or restarting the web server, the site goes down
- **Limited scalability:** Cannot handle large amounts of incoming traffic

## General Requirements

- Each task requires a whiteboard diagram (can be drawn on paper, whiteboard, or digital tool)
- Take a picture/screenshot of your diagram
- Upload the image to an image hosting service
- Insert the link to the image in the answer file
- Push your answer file to GitHub
- Insert the GitHub file link into the submission field

## Resources

Read or watch:
- Network basics
- Server
- Web server
- DNS
- Load balancer
- Monitoring
- Database
- Single point of failure
- How to avoid downtime when deploying new code
- High availability cluster (active-active/active-passive)
- What is HTTPS
- What is a firewall

## Author

This project is part of the Holberton School System Engineering & DevOps curriculum.

## Repository Structure

```
holbertonschool-system_engineering-devops/
└── web_infrastructure_design/
    ├── README.md
    └── 0-simple_web_stack
```

## How to Use

1. Review the requirements for each task
2. Design the infrastructure on a whiteboard or diagramming tool
3. Take a screenshot/photo of your design
4. Upload to an image hosting service (e.g., Imgur, GitHub, etc.)
5. Add the image URL to the corresponding task file
6. Commit and push your changes to GitHub
