---
title: "Event 1"
date: 2026-06-06
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---



# Summary Report: “AWS Study Group Meetup – Technology, Cloud, Security, AI, and Career Development”

### Event Objectives

- Introduce practical technologies used in modern software development and cloud computing.
- Share knowledge about Docker, AWS security, WebSocket-based multiplayer systems, teamwork, GraphRAG, and career development.
- Help participants understand how AWS services can be applied to real projects.
- Provide learning directions for students interested in Cloud, DevOps, Cybersecurity, Artificial Intelligence, and System Administration.
- Create opportunities for participants to learn from speakers with different technical backgrounds.

### Speakers

- **Bao Huynh** – Speaker of the Docker and containerization session
- **Le Hoang Gia Dai** – Speaker of the Machine Learning-based Network Intrusion Detection System on AWS session
- **Nguyen Quoc Bao** – Speaker of the Godot multiplayer and AWS WebSocket session
- **Truong Huy Phuoc** – Speaker of the effective teamwork session
- **Viet Phat** – Speaker of the GraphRAG with Amazon Bedrock and Amazon Neptune session
- **Tran Trung Vinh** – System Administrator at Central Retail Group and speaker of the IT Helpdesk to Senior Sysadmin session

### Key Highlights

#### Docker – A Containerization Technology

The first session introduced Docker and the role of containerization in modern application development.

- Virtual machines provide complete operating-system environments, while containers share the host operating system and are generally lighter.
- Docker images are reusable templates containing application code, libraries, and dependencies.
- Docker containers are running instances created from Docker images.
- Dockerfiles describe the steps required to build an image.
- Image layers allow Docker to reuse unchanged parts of an image and improve build speed.
- Docker can help teams maintain consistent development, testing, and deployment environments.
- Common use cases include microservices, CI/CD pipelines, application testing, and cloud deployment.

This session helped me understand why containers are widely used in cloud-native systems and how Docker reduces differences between development and production environments.

#### Machine Learning-based Network Intrusion Detection System on AWS

The second session focused on improving network security by combining AWS services with Machine Learning.

- AWS WAF can protect web applications and APIs from common threats such as SQL Injection, Cross-Site Scripting, bots, and brute-force attempts.
- Rule-based systems are useful but may have difficulty detecting new or unusual attack patterns.
- A Machine Learning-based Network Intrusion Detection System can analyze traffic and identify abnormal behavior.
- The CSE-CIC-IDS2018 dataset was introduced as a source of normal and malicious network traffic.
- Important data-processing steps include cleaning data, selecting useful features, handling missing values, and addressing class imbalance.
- LightGBM was presented as a possible model for classifying network traffic.
- Evaluation methods such as accuracy, precision, recall, F1-score, and confusion matrix are important when assessing a security model.
- AWS services can support data storage, processing, model deployment, logging, and monitoring.

This topic was especially relevant to my cybersecurity studies because it showed how traditional security controls and Machine Learning can complement each other.

#### Multiplayer in the Cloud – Connecting Godot Clients with AWS WebSockets

The third session presented a serverless architecture for connecting Godot game clients through AWS WebSockets.

- UDP and ENet are suitable for fast real-time gameplay but may require more infrastructure management.
- WebSockets provide persistent two-way communication between clients and servers.
- WebSockets are suitable for chat systems, game lobbies, turn-based games, status updates, and notifications.
- Amazon API Gateway WebSocket can manage client connections.
- AWS Lambda can process connection, disconnection, and message events.
- Amazon DynamoDB can store connection IDs and simple player-state information.
- Amazon CloudWatch can store logs and support troubleshooting.
- The architecture must handle stale connections, Lambda statelessness, table-scan costs, and disconnected clients.

This session helped me understand how serverless AWS services can be combined to create a simple real-time application without maintaining a traditional server.

#### The Art of Effective Teamwork

The fourth session focused on the human and organizational factors that influence project success.

The speaker presented four important principles:

- **Clear and Shared Goals:** Team members should understand the expected result and work toward the same objective.
- **Right Person, Right Place:** Tasks should be assigned based on each member's strengths and experience.
- **Open Communication and Active Listening:** Team members should communicate honestly, listen carefully, and provide constructive feedback.
- **Personal Accountability:** Each member should take responsibility for assigned tasks and deadlines.

The session also introduced collaboration tools such as Trello, ClickUp, Google Workspace, Slack, and Discord.

The main lesson was that tools can support teamwork, but they cannot replace clear communication, responsibility, and mutual respect.

#### Build GraphRAG Applications Using Amazon Bedrock and Amazon Neptune

The fifth session introduced Retrieval-Augmented Generation and GraphRAG.

- Traditional RAG retrieves relevant text and provides it to a Large Language Model before generating an answer.
- Traditional RAG may have difficulty answering questions that require reasoning across several connected entities.
- GraphRAG represents knowledge using nodes, edges, and relationships.
- Graph traversal can support multi-hop reasoning and improve relationship awareness.
- Amazon Bedrock Knowledge Bases can support document processing, chunking, embeddings, and retrieval.
- Amazon Neptune can store and process graph data.
- Cypher queries can be used to search relationships in a knowledge graph.
- Two implementation approaches were introduced:
  - A managed approach using Amazon Bedrock Knowledge Bases and Neptune Analytics
  - A custom approach using LlamaIndex and Amazon Neptune

This session helped me understand that GraphRAG is useful when the relationships between pieces of information are as important as the information itself.

#### From IT Helpdesk to Senior Sysadmin

The final session focused on career development from IT Helpdesk to System Administrator and later to Cloud or DevOps roles.

- IT Helpdesk helps develop troubleshooting, communication, user-support, and problem-solving skills.
- Linux and networking are important foundations for System Administration.
- Building a personal lab is an effective way to practice server, network, and security skills.
- A System Administrator may be responsible for:
  - Server and network management
  - Security patching
  - Monitoring
  - Capacity planning
  - Documentation and runbooks
  - Automation of repetitive tasks
- Cloud and DevOps learning paths may include AWS, Terraform, Docker, Infrastructure as Code, and CI/CD.
- Practical projects and a strong portfolio are valuable when applying for technical positions.
- Learners should focus deeply on a small number of core skills instead of learning many tools without enough practice.

This session provided a realistic career roadmap and showed how Helpdesk experience can become a foundation for more advanced infrastructure roles.

### Key Takeaways

#### Technical Knowledge

- Docker helps package applications and dependencies into consistent, portable environments.
- Security systems can combine rule-based protection with Machine Learning-based anomaly detection.
- AWS serverless services can support real-time applications through API Gateway, Lambda, DynamoDB, and CloudWatch.
- GraphRAG can improve information retrieval when questions depend on relationships between entities.
- Linux, networking, automation, and cloud knowledge are important foundations for infrastructure careers.

#### Architecture and Cloud Services

- Each AWS service should be selected according to the problem being solved.
- Serverless services reduce infrastructure-management work but still require careful design and monitoring.
- CloudWatch is important for observing system behavior and troubleshooting errors.
- DynamoDB is useful for simple state and connection information, but inefficient scans should be avoided.
- Security models should be evaluated using appropriate metrics rather than accuracy alone.

#### Teamwork and Career Development

- Clear objectives and personal responsibility improve team performance.
- Technical tools are most effective when the team communicates openly.
- Building personal projects and labs is an effective way to strengthen practical skills.
- A good career roadmap should start with strong foundations before moving to advanced tools.
- Continuous learning is necessary because cloud, security, and artificial intelligence technologies change quickly.

### Applying to Work

After the event, I identified several practical ways to apply the knowledge to my studies and projects:

- Use Docker to create a consistent environment for backend and cloud projects.
- Practice writing a simple Dockerfile and running an application inside a container.
- Review network-security datasets and learn basic data-processing techniques using Python.
- Compare traditional rule-based detection with Machine Learning-based anomaly detection.
- Use Amazon CloudWatch to review logs, metrics, and errors in AWS projects.
- Study API Gateway WebSocket and Lambda for chat, notification, or real-time status features.
- Use DynamoDB carefully for storing simple connection or session information.
- Apply clear task assignment and regular progress updates in team projects.
- Use Trello, ClickUp, or another task-management tool to track responsibilities.
- Learn the fundamentals of RAG before experimenting with GraphRAG.
- Create a small knowledge graph to understand nodes, edges, and graph queries.
- Strengthen Linux, networking, troubleshooting, and documentation skills.
- Build a personal lab and record the configuration steps in a portfolio.
- Continue learning AWS, Docker, automation, and Infrastructure as Code.

### Event Experience

Attending this meetup was valuable because the event covered several different areas instead of focusing on only one technology.

#### Learning from Different Technical Topics

The Docker session provided a clear introduction to containers and their role in application deployment. The cybersecurity session connected AWS security services with Machine Learning, which was closely related to my field of study. The WebSocket session showed how multiple AWS services can work together in a real-time system.

The GraphRAG session introduced a newer AI architecture and helped me understand why relationships between data entities can improve retrieval. The System Administrator session provided a practical career roadmap that connected IT Helpdesk, infrastructure, cloud, and DevOps skills.

#### Understanding the Importance of Teamwork

The teamwork session reminded me that technical knowledge alone is not enough for a successful project. Team members also need shared goals, open communication, appropriate task assignments, and personal accountability.

This is useful for both academic projects and professional work because many technical problems require cooperation between people with different responsibilities.

#### Career Direction

The event helped me better understand several possible career directions, including:

- Cloud Engineer
- DevOps Engineer
- Cybersecurity Engineer
- System Administrator
- Backend or Serverless Developer
- Artificial Intelligence Engineer

The final session was particularly helpful because it showed that career development is a gradual process. Strong troubleshooting, Linux, networking, documentation, and practical project experience can create a foundation for more advanced cloud and DevOps roles.

#### Lessons Learned

- Learning should include both theory and practical exercises.
- Small personal projects can help turn workshop knowledge into real skills.
- Monitoring, security, documentation, and teamwork should be considered from the beginning of a project.
- It is better to understand a few core technologies clearly than to study many tools only at a surface level.
- Cloud services are most useful when they are selected according to real project requirements.

### Some Event Photos

*Add your event photos here.*
![Event photo 1](/images/event-participated/img1.jpg)

![Event photo 2](/images/event-participated/img2.jpg)

![Event photo 3](/images/event-participated/img3.jpg) 

> Overall, the event gave me a broader understanding of modern software development, cloud architecture, cybersecurity, artificial intelligence, teamwork, and career development. It also helped me identify practical topics that I can continue studying and applying to future AWS and cybersecurity projects.