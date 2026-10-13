# Module 1: DevOps Engineering Assignment

## Project Overview

This repository contains my Module 1 DevOps Engineering assignment.

It includes theoretical answers, scenario-based solutions, a local demo web application, and practical documentation for exposing the application through ngrok.

## Objectives

- Understand DevOps principles and responsibilities.
- Explain the role of DevOps in the Software Development Life Cycle.
- Apply basic troubleshooting and incident management practices.
- Run a web application locally.
- Expose a local application using ngrok.
- Document the work using GitHub.

## Repository Structure

```text
.
├── README.md
├── app/
│   └── index.html
├── screenshots/
│   ├── 01-local-application.png
│   ├── 02-ngrok-public-url.png
│   ├── 03-ngrok-public-access.png
│   └── 04-github-repository.png
└── .gitignore
.
## Part A: Theoretical Questions

1. What is DevOps Engineering? How does it differ from traditional development and operations roles?

DevOps Engineering is an approach that connects software development with IT operations to make software delivery more efficient. It combines teamwork, automation, and modern tools to help organizations develop, test, and release applications with fewer problems.

In a traditional working environment, developers are mainly responsible for writing code, while the operations team manages servers, deployments, and system maintenance. Since these teams often work independently, resolving issues can take longer.

DevOps reduces this gap by encouraging both teams to share responsibilities. It also uses automated workflows, continuous integration, continuous delivery, and performance monitoring to improve the overall software delivery process.

2. How does DevOps fit into the Software Development Life Cycle (SDLC)?

DevOps contributes to different stages of the Software Development Life Cycle (SDLC) and helps teams manage software from initial planning through ongoing maintenance.

Some important stages where DevOps provides benefits are:

* Development: Version control systems such as Git help developers track changes and work together on the same project.
* Testing: Automated testing makes it easier to identify bugs before the software reaches users.
* Deployment: CI/CD tools help automate application builds and releases, reducing manual work.
* Monitoring and Maintenance: Monitoring systems provide information about application performance and help teams detect problems quickly.

By connecting these stages, DevOps creates a continuous improvement process in which feedback from one stage helps improve the next.

3. What values does a DevOps Engineer bring to an organization? Explain any four.

A DevOps Engineer can improve an organization’s efficiency, software quality, and service reliability in several ways.

1. Automation

Automation reduces the need for repetitive manual tasks and helps maintain consistency. For instance, a pipeline can automatically build an application, run tests, and deploy a new version.

2. Better Teamwork

DevOps encourages developers, operations engineers, and security professionals to work toward common goals. When a deployment problem occurs, these teams can investigate and resolve it together.

3. Improved System Reliability

Monitoring tools, regular backups, automated checks, and recovery plans help keep applications available. These practices also make it easier to detect failures before they cause major disruption.

4. Efficient Software Delivery

DevOps practices allow organizations to deliver software updates more regularly. Automated workflows and testing help teams introduce improvements without relying entirely on lengthy manual procedures.

4. Why is prior Software Engineering (SWE) experience helpful before becoming a DevOps Engineer?

Experience in Software Engineering provides a useful foundation for understanding how applications are developed and operated. It helps a DevOps Engineer understand source code, application architecture, software dependencies, testing methods, and debugging techniques.

For example, an application may fail during deployment because a required library is missing or a configuration is incorrect. Someone familiar with software development may find it easier to understand the error and work with developers to correct it.

However, a Software Engineering background is not essential for every DevOps position. Professionals with experience in networking, Linux administration, infrastructure management, or cloud computing can also develop the skills needed for a DevOps career.

5. Why is networking knowledge important for DevOps roles?

Networking knowledge helps DevOps Engineers understand how applications communicate with servers, containers, databases, and cloud-based services.

Several networking concepts are particularly important:

* DNS: Translates domain names into IP addresses so systems can locate the correct services.
* IP Addressing: Provides addresses that allow devices and servers to communicate across networks.
* Ports: Identify specific services running on a system. For example, HTTPS commonly uses TCP port 443.
* Network Protocols: Protocols such as TCP, UDP, HTTP, and HTTPS define how information is transmitted between systems.

Consider a situation where users cannot access a web application. A DevOps Engineer may need to check DNS records, firewall policies, routing, network connectivity, and the application’s listening port to identify the source of the problem.

6. What soft skills are essential for a DevOps Engineer?

Technical knowledge alone is not enough to succeed in DevOps. Engineers also need interpersonal and organizational skills to work effectively with different teams.

Important soft skills include:

* Communication: Explaining technical issues clearly and providing timely updates.
* Teamwork: Cooperating with developers, system administrators, security teams, and managers.
* Analytical Thinking: Examining evidence and identifying the underlying cause of a technical issue.
* Adaptability: Learning unfamiliar technologies and adjusting to new requirements.
* Time Management: Managing routine responsibilities while giving priority to urgent incidents.

For example, when a production service fails, an engineer must communicate the situation clearly while coordinating troubleshooting activities. Good communication helps everyone understand their responsibilities and work toward a solution.

7. Explain the importance of patience and troubleshooting mindset with a real-life example.

Patience and a structured troubleshooting approach are important because technical problems do not always have an obvious cause. Making changes without understanding the issue can create additional problems.

For example, imagine that a web application stops responding immediately after a software update. Rather than repeatedly restarting the server, the DevOps Engineer should examine the application logs, system resources, service status, network connections, and recent configuration changes.

After collecting sufficient information, the engineer can identify the likely cause, apply a suitable correction, and test whether the application is working normally again.

This method helps reduce downtime, avoids unnecessary changes, and provides useful information for preventing similar incidents in the future.

## Part B: Scenario-Based Questions

1. A new student is unfamiliar with GitHub and cloud platforms. How would you onboard the student efficiently?

I would follow a structured onboarding process.

1. Introduction: Explain the course objectives, required tools, and expected outcomes.
2. Tool Setup: Help the student create a GitHub account and install Git.
3. Basic Training: Introduce repositories, commits, branches, pull requests, and README files.
4. Cloud Fundamentals: Explain basic cloud concepts such as virtual machines, storage, networking, and identity management.
5. Documentation: Share official documentation, setup instructions, and example projects.
6. Communication: Introduce the team’s communication channels and explain where to ask technical questions.
7. Hands-on Practice: Ask the student to create a small repository, commit a file, and document the work.
8. Feedback: Review progress and provide additional support where necessary.

This approach helps the student learn the required tools through practical experience.

2. An application goes down unexpectedly during a production deployment. How would you troubleshoot it?

I would follow these steps:

Step 1: Assess the Impact

Confirm the outage, identify affected services, and determine how many users are impacted.

Step 2: Communicate

Notify the relevant team members and stakeholders through the incident communication channel.

Step 3: Check Monitoring and Logs

Review application logs, system logs, CPU and memory usage, network connectivity, and monitoring alerts.

Step 4: Identify Recent Changes

Check the latest deployment, configuration updates, dependency changes, and infrastructure modifications.

Step 5: Restore Service

If the new release is responsible and rollback is safe, restore the last known working version using the established rollback procedure.

Step 6: Verify Recovery

Test the application, check its health endpoints, and confirm that users can access it successfully.

Step 7: Conduct Root Cause Analysis

After recovery, investigate the underlying cause and document corrective and preventive actions.

The priority is to restore service safely, communicate clearly, and prevent recurrence.

3. How can DevOps balance frequent releases with system stability?

DevOps practices can improve both release speed and reliability.

* CI/CD Pipelines: Automate builds, tests, and deployments.
* Automated Testing: Detect defects before production deployment.
* Code Reviews: Improve code quality and reduce avoidable mistakes.
* Staging Environments: Test changes in an environment similar to production.
* Monitoring and Alerting: Detect failures and performance degradation quickly.
* Gradual Releases: Use canary deployments or blue-green deployments where appropriate.
* Rollback Procedures: Restore a previous stable version when a release fails.
* Post-Incident Reviews: Identify weaknesses and improve future releases.

These practices help teams release features frequently without sacrificing reliability.

4. How can proper onboarding to communication platforms improve distributed DevOps workflows?

Distributed teams need clear and consistent communication.

During onboarding, team members should learn which platforms are used for daily communication, technical discussions, incident alerts, documentation, and task tracking.

For example, a team may use Slack or Microsoft Teams for communication, Jira for task tracking, GitHub for code collaboration, and a shared documentation platform for operational procedures.

The team should also define incident severity levels, escalation procedures, and responsibilities.

This reduces confusion, speeds up incident response, and ensures that everyone can access the information needed to perform their tasks.
