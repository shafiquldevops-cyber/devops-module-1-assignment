# Module 1: DevOps Engineering Assignment

## Project Overview

This repository contains my Module 1 DevOps Engineering assignment.

It includes theoretical answers, scenario-based solutions, a local demo web application, and practical documentation for exposing the application through ngrok.

## Objectives

- Understand DevOps principles and responsibilities.
- Explain the role of DevOps in the Software Development Life Cycle.
- Apply troubleshooting and incident management practices.
- Run a web application locally.
- Expose a local application using ngrok.
- Document the work using GitHub.

## Repository Structure

```text
devops-module-1-assignment/
├── README.md
├── app/
│   └── index.html
├── screenshots/
│   ├── 01-local-application.png
│   ├── 02-ngrok-public-url.png
│   └── 03-ngrok-public-access.png
└── .gitignore
```


## Part A: Theoretical Questions

1. What is DevOps Engineering? How does it differ from traditional development and operations roles?

DevOps Engineering combines practices, tools, automation, and cultural principles to improve collaboration between software development and IT operations teams.

In traditional environments, developers and operations teams may work separately. DevOps encourages shared responsibility, continuous integration, continuous delivery, automated testing, monitoring, and collaboration.

2. How does DevOps fit into the Software Development Life Cycle (SDLC)?

DevOps supports the SDLC from planning and development through testing, deployment, monitoring, and maintenance.

* Development: Version control tools such as Git help manage code changes.
* Testing: Automated testing identifies defects before release.
* Deployment: CI/CD pipelines automate application delivery.
* Monitoring: Monitoring tools identify performance issues and failures.

3. What values does a DevOps Engineer bring to an organization? Explain four values.

Automation: Automating repetitive tasks reduces manual errors and saves time. For example, a CI/CD pipeline can automatically test application changes.

Collaboration: DevOps encourages developers, operations teams, and security teams to work together.

Reliability: Monitoring, testing, backups, and recovery procedures help maintain service availability.

Faster Delivery: Automated pipelines help teams release software changes more frequently and consistently.

4. Why is prior Software Engineering experience helpful before becoming a DevOps Engineer?

Software Engineering experience helps DevOps Engineers understand application architecture, dependencies, testing, debugging, and build processes.

For example, knowledge of application dependencies can help troubleshoot a deployment failure caused by a missing package. However, prior software development experience is helpful rather than mandatory for every DevOps role.

5. Why is networking knowledge important for DevOps roles?

Networking knowledge helps engineers troubleshoot communication between applications, servers, containers, and cloud services.

* DNS resolves domain names to IP addresses.
* IP addressing identifies devices and network interfaces.
* Ports identify network endpoints used by applications.
* Protocols such as HTTP, HTTPS, TCP, and UDP define communication methods.

For example, a failed connection may be caused by DNS resolution, firewall rules, or a service listening on the wrong port.

6. What soft skills are essential for a DevOps Engineer?

Important soft skills include communication, teamwork, problem-solving, adaptability, and time management.

During an incident, clear communication helps team members coordinate troubleshooting, share updates, assign responsibilities, and inform stakeholders.

7. Explain the importance of patience and troubleshooting mindset with a real-life example.

Patience helps engineers investigate problems systematically rather than applying random fixes.

For example, if an application becomes unavailable after deployment, the engineer should review logs, service status, resource usage, network connectivity, and recent changes. After identifying the cause, the engineer can apply a suitable fix and verify recovery.

Part B: Scenario-Based Questions

1. How would you onboard a new student unfamiliar with GitHub and cloud platforms?

I would provide a structured onboarding process.

1. Explain the course objectives and required tools.
2. Help the student create a GitHub account and install Git.
3. Teach repositories, commits, branches, and README files.
4. Introduce cloud fundamentals such as virtual machines, storage, and networking.
5. Share official documentation and practical examples.
6. Explain communication channels and where to ask questions.
7. Assign a small hands-on project and review the student’s progress.

This approach combines documentation, practical exercises, and communication to help the student learn efficiently.

2. How would you troubleshoot an application outage during production deployment?

1. Assess the outage and identify affected users and services.
2. Notify the incident response team and relevant stakeholders.
3. Review application logs, system metrics, and monitoring alerts.
4. Investigate recent deployments and configuration changes.
5. If the release caused the outage, consider a safe rollback to the last known working version.
6. Verify application health and user accessibility.
7. Document the root cause and implement preventive actions.

The main priorities are safe service restoration, clear communication, and preventing recurrence.

3. How can DevOps balance frequent releases with system stability?

DevOps can balance release speed and stability through automated testing, CI/CD pipelines, code reviews, staging environments, monitoring, and rollback procedures.

Canary or blue-green deployments can reduce risk by gradually introducing changes. Post-incident reviews help teams identify weaknesses and improve reliability.

4. How can onboarding to communication platforms improve distributed DevOps workflows?

Proper onboarding helps team members understand where to communicate, report incidents, document decisions, and track tasks.

For example, teams may use Microsoft Teams or Slack for communication, GitHub for code collaboration, and Jira for task management.

Clear incident channels, escalation procedures, and role assignments reduce confusion and improve response times.

Part C: Technical / Practical Tasks

Task 1: Local DevOps Demo Application

Objective: Run a simple web application locally and verify that it works.

Tools Used:

* macOS
* Python 3
* HTML
* Python HTTP Server

Application File: app/index.html

Command Used:

python3 -m http.server 8000 --bind 127.0.0.1 --directory app

Local URL: http://127.0.0.1:8000

Verification:

The application was opened in a web browser to verify that the local web server was serving the demo page.

Screenshot:

Why is local testing important in DevOps?

Local testing helps developers verify application behavior before deployment. It allows early detection of errors and reduces the risk of introducing defects into production environments.

Task 2: Exposing the Local Application Using ngrok

Objective: Make the local demo application accessible through a public HTTPS URL.

Tool Used: ngrok

Local Application: http://127.0.0.1:8000

Command Used:

ngrok http 8000

Public URL: https://overlook-bristle-faster.ngrok-free.dev/

Verification:

The public URL was opened in a web browser to verify access to the application through the ngrok tunnel.

Screenshot 1: ngrok Tunnel

Screenshot 2: Public Application Access

Real-World Use Case:

ngrok can help developers share a locally running application with teammates or clients for testing and feedback without deploying it to a public production server.


Conclusion

This assignment demonstrates basic DevOps concepts, troubleshooting practices, local application testing, network accessibility, ngrok tunneling, and GitHub documentation.
