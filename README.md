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

Part A: Theoretical Questions

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

Part B: Scenario-Based Questions

1. A new student is unfamiliar with GitHub and cloud platforms. How would you onboard the student efficiently?

I would introduce the student to the required tools gradually, combining basic explanations with practical exercises.

Step 1: Explain the Learning Objectives

Start by describing the purpose of the training, the tools involved, and the skills the student is expected to develop.

Step 2: Prepare the Development Environment

Help the student create a GitHub account, install Git, and configure the necessary software.

Step 3: Introduce GitHub Fundamentals

Demonstrate how repositories, commits, branches, pull requests, and README files are used in collaborative projects.

Step 4: Cover Basic Cloud Concepts

Explain the role of virtual machines, cloud storage, networking, and identity management. Use simple examples to show how these services work.

Step 5: Provide Learning Resources

Share official documentation, setup guides, and beginner-friendly project examples so the student can continue learning independently.

Step 6: Explain Team Communication

Show the student how to communicate with team members, report technical difficulties, and find answers to common questions.

Step 7: Assign a Practical Exercise

Ask the student to create a repository, add a sample file, commit a change, and write a short project description.

Step 8: Review Progress

Check the student’s work, identify areas that need improvement, and provide additional guidance.

This process helps beginners become familiar with the tools while building confidence through hands-on practice.

2. An application goes down unexpectedly during a production deployment. How would you troubleshoot it?

I would approach the incident systematically, focusing first on restoring the service and then identifying the underlying cause.

Step 1: Determine the Scope of the Problem

Check whether the application is completely unavailable or whether only certain features or users are affected.

Step 2: Inform the Relevant People

Notify the responsible technical team and other stakeholders through the established incident communication channel.

Step 3: Examine Logs and Monitoring Data

Review application errors, server logs, CPU and memory consumption, network status, and monitoring alerts to identify unusual behaviour.

Step 4: Review Recent Changes

Investigate whether the latest release introduced a code defect, configuration problem, dependency conflict, or infrastructure issue.

Step 5: Recover the Application

If the new deployment is identified as the likely cause, consider rolling back to the previous stable version, provided the rollback procedure is safe and appropriate.

Step 6: Confirm That the Service Is Working

Test the application, check its health status, and verify that users can access the expected functionality.

Step 7: Investigate the Root Cause

Once the service has recovered, document the incident, determine why it happened, and identify changes that could prevent a recurrence.

The main objective is to minimize service disruption while ensuring that recovery actions are safe and properly communicated.

3. How can DevOps balance frequent releases with system stability?

DevOps can support frequent software releases without compromising stability by combining automation, testing, controlled deployments, and continuous monitoring.

The following practices are particularly useful:

* CI/CD Automation: Automates repetitive build, testing, and deployment activities.
* Automated Testing: Identifies software defects before they affect production users.
* Code Review: Allows team members to examine changes and identify potential problems before merging them.
* Staging Environment: Provides a separate environment for validating releases before production deployment.
* Continuous Monitoring: Helps engineers detect errors, performance issues, and service interruptions.
* Controlled Deployment: Techniques such as canary and blue-green deployments reduce the risk associated with releasing changes to all users at once.
* Rollback Planning: Makes it possible to return to a stable version when a new release causes problems.
* Post-Incident Analysis: Helps teams learn from failures and improve their development and deployment processes.

When these practices are implemented properly, organizations can release improvements more frequently while maintaining dependable services.

4. How can proper onboarding to communication platforms improve distributed DevOps workflows?

Distributed DevOps teams often work from different locations and time zones. A clear communication process helps them coordinate tasks, exchange technical information, and respond to incidents without unnecessary delays.

During onboarding, new team members should learn which platforms are used for different activities. For example, Slack or Microsoft Teams may be used for discussions, Jira for tracking tasks, GitHub for code collaboration, and a shared documentation system for recording technical procedures.

The team should also establish clear guidelines for reporting incidents, assigning responsibilities, escalating urgent issues, and sharing progress updates.

For instance, if a production server becomes unavailable, the responsible engineer should know where to report the incident, whom to notify, and where to document troubleshooting results.

A well-organized communication process reduces misunderstandings, improves coordination, and helps distributed teams resolve technical issues more efficiently.
