# 🧾 AWS Advanced Services – Complete Notes

---

## 🌐 1. Route 53

### Overview:

Amazon Route 53 is a **highly available and scalable Domain Name System (DNS)** web service.

### Key Features:

* **Domain Registration**: Buy/manage domains directly.
* **DNS Service**: Translate domain names to IP addresses.
* **Health Checks**: Monitor endpoints and route traffic away from unhealthy resources.
* **Routing Policies**:

  * Simple Routing
  * Weighted Routing
  * Latency-based Routing
  * Failover Routing
  * Geolocation Routing

### Use Case:

Distribute traffic across global resources, domain management, high-availability setup.

---

## 📢 2. SNS (Simple Notification Service)

### Overview:

SNS is a **fully managed messaging service** for decoupled microservices, distributed systems, and serverless apps.

### Core Concepts:

* **Topics**: Named communication channels.
* **Subscribers**: Endpoints like Lambda, SQS, Email, SMS.
* **Publishers**: Send messages to topics.

### Use Case:

* Send alerts (e.g., CloudWatch alarms)
* Event-driven architecture
* Fan-out pattern

---

## ⏱️ 3. CloudWatch

### Overview:

Amazon CloudWatch monitors **resources and applications** in real time.

### Key Components:

* **Metrics**: CPU, Memory, etc.
* **Logs**: Collect and monitor logs.
* **Alarms**: Trigger actions (SNS, Auto Scaling) when thresholds are breached.
* **Dashboards**: Custom visualizations of metrics.

### Use Case:

Track EC2 health, set alarms for scaling, aggregate logs from ECS, Lambda, etc.

---

## 📬 4. SQS (Simple Queue Service)

### Overview:

SQS is a **fully managed message queuing service** that decouples components of a distributed system.

### Queue Types:

* **Standard Queue**: Best-effort ordering, at-least-once delivery.
* **FIFO Queue**: Guaranteed order, exactly-once delivery.

### Use Case:

* Buffering requests between microservices
* Decouple tasks from users (async processing)

---

## 🕵️ 5. CloudTrail

### Overview:

AWS CloudTrail enables **governance, compliance, and auditing** by recording AWS API calls.

### Features:

* Tracks user actions via console, SDKs, CLI
* Delivered to S3 and viewable in CloudTrail console
* Supports CloudWatch integration

### Use Case:

Security audits, troubleshooting, compliance reporting.

---

## 🛠 6. CloudFormation

### Overview:

CloudFormation is an **Infrastructure as Code (IaC)** service.

### Key Features:

* Create AWS resources using templates (JSON/YAML)
* Supports parameters, mappings, conditionals
* Stack updates, rollback, drift detection

### Use Case:

Automate entire environments (e.g., VPC + EC2 + RDS)

---

## ⚖️ 7. ELB (Elastic Load Balancer)

### Types:

* **Application Load Balancer (ALB)** – HTTP/HTTPS
* **Network Load Balancer (NLB)** – TCP/UDP
* **Gateway Load Balancer (GWLB)** – for third-party appliances
* **Classic Load Balancer (CLB)** – legacy support

### Use Case:

Distribute incoming application or network traffic to targets like EC2, ECS, Lambda.

---

## 🔍 8. AWS Config

### Overview:

A service to **assess, audit, and evaluate** resource configurations.

### Features:

* Detect drift from desired state
* Record resource configuration history
* Rule-based compliance evaluation

### Use Case:

Track configuration changes, ensure compliance.

---

## 🔐 9. AWS Secrets Manager

### Overview:

Stores, manages, and retrieves **secrets** (e.g., API keys, DB passwords).

### Features:

* Secret rotation
* Encryption with KMS
* Fine-grained IAM access

### Use Case:

Secure credential storage, dynamic secret rotation.

---

## ⚙️ 10. Systems Manager Parameter Store

### Overview:

Secure storage for **configuration data and secrets**.

### Features:

* Plaintext and encrypted parameters
* Versioning
* IAM control

### Use Case:

Manage app configs, pass parameters to EC2/Lambda.

---

## 📜 11. AWS Certificate Manager (ACM)

### Overview:

Provision, manage, and deploy **SSL/TLS certificates**.

### Features:

* Free public SSL certs for AWS services
* Auto renewal
* Integrated with ELB, CloudFront, API Gateway

### Use Case:

Secure websites or APIs with HTTPS easily.

---

## 💰 12. AWS Cost Explorer

### Overview:

Analyze **AWS usage and cost patterns**.

### Features:

* Visual dashboards for cost tracking
* Filters by service, region, tag
* Forecasting & budgeting support

### Use Case:

Cost optimization, budget tracking, anomaly detection.

---

## 📊 13. AWS Budgets

### Overview:

Set **custom cost and usage budgets** and get alerts.

### Features:

* Alerts via email/SNS
* Supports RI/SP usage and savings plans
* Tracks against forecasts

### Use Case:

Avoid overspending, enforce budget compliance.

---

## 🌍 14. AWS CloudFront

### Overview:

A **Content Delivery Network (CDN)** that delivers content with low latency.

### Features:

* Global edge locations
* Integrated with S3, ELB, and custom origins
* Caching, signed URLs

### Use Case:

Speed up website/static content delivery, secure APIs.

---

## 🏢 15. AWS Organizations

### Overview:

Manage **multiple AWS accounts centrally**.

### Features:

* Consolidated billing
* SCPs (Service Control Policies)
* OUs (Organizational Units)

### Use Case:

Enterprise account management, billing separation, policy enforcement.

---

## 🛡 16. AWS WAF (Web Application Firewall)

### Overview:

Protects applications from **common web exploits**.

### Features:

* Define rules to block/allow traffic
* Bot control, rate limiting
* Integrated with CloudFront, ALB, API Gateway

### Use Case:

Secure web apps from SQL injection, XSS, DDoS attempts.

---

## 🛡️ 17. AWS Shield

### Overview:

**DDoS protection service** for applications.

### Types:

* **Standard**: Free, automatic
* **Advanced**: Enhanced protection, cost protection, 24/7 DDoS response team

### Use Case:

Secure public-facing apps like websites, APIs.

---

## 🧠 18. AWS Trusted Advisor

### Overview:

Provides **real-time best practice checks**.

### Categories:

* Cost optimization
* Security
* Fault tolerance
* Performance
* Service limits

### Use Case:

Improve resource utilization, security posture, reliability.
