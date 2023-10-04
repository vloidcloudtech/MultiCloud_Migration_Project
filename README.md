# Hands-on Project Presentation: MultiCloud Migration Mastery

Greetings! Today, I am thrilled to walk you through my successful execution of a MultiCloud migration project involving Amazon Web Services (AWS) and Google Cloud Platform (GCP). Let's delve into the intricacies of seamless cloud migration!

Here is the blog post I made breaking down this project. (https://medium.com/@vloidcloudtech/hands-on-project-implementation-mission-accomplished-in-multicloud-architecture-94160edf48d0)
---

## Mission 1: Setting Up AWS Infrastructure

### 1.1 Access AWS Console and User Creation

Creating a programmatic user named `terraform-en-1` ensures secure access to AWS services. The attached policy `AmazonS3FullAccess` grants the necessary permissions for handling S3 resources programmatically, a fundamental step in cloud storage setup.

### 1.2 Key Management and Security Best Practices

Generating access keys for `terraform-en-1` and storing them securely in `accessKeys.csv` is essential. These keys serve as authentication tokens, allowing secure communication between the cloud environment and the user’s local system. Adhering to security best practices prevents unauthorized access and potential breaches.

### 1.3 AWS Environment Preparation

- **Shell Script Execution:** The provided scripts automate environment setup tasks, ensuring consistency and reducing manual errors.
  
- **AWS and GCP Configuration:** Setting AWS credentials and enabling necessary GCP APIs ensures seamless interaction between AWS and GCP services, paving the way for cross-cloud functionality.

---

## Mission 2: Building Applications on AWS and GCP

### 2.1 AWS Setup

Creating another user, e.g., `luxxy-covid-testing-system-en-app1`, allows controlled access to S3 resources. Following the principle of least privilege, this user is granted `AmazonS3FullAccess` only, limiting access rights to the minimum necessary for the task.

### 2.2 GCP Setup

- **Database User Creation:** The `app` user is specifically created for interacting with the Cloud SQL MySQL database, ensuring that application components have distinct access points, enhancing security.

- **File Download and Database Schema Setup:** Fetching mission2 files and importing the SQL schema sets the groundwork for application deployment. Establishing the database schema ensures consistent data organization, vital for functional applications.

### 2.3 Docker Image Build and Deployment

- **Containerization:** Building a Docker image allows for consistent deployment across different cloud platforms. The image is then pushed to Google Container Registry, a centralized repository for managing Docker images.

- **Kubernetes Deployment Configuration:** Modifying the Kubernetes deployment file (`luxxy-covid-testing-system.yaml`) customizes the application’s runtime environment. Environment-specific variables such as project IDs, database credentials, and IP addresses are adjusted, ensuring seamless integration with the respective cloud services.

---

## Mission 3: MultiCloud Data Migration

### 3.1 GCP Database Migration

Downloading mission3 files and importing the SQL dump to the Cloud SQL MySQL database establishes data continuity. Ensuring successful migration verifies that the application’s data layer is intact and functional, a critical aspect of any migration process.

### 3.2 AWS PDF Files Migration

Syncing PDF files with the designated S3 bucket finalizes the data migration process. Rigorous testing ensures the integrity of the migrated data, confirming that all components, including static files, are successfully transitioned.

---

## Key Takeaways:

- **Security First:** Adhering to the principle of least privilege and employing secure key management practices ensures data confidentiality and system integrity.
  
- **Automation for Consistency:** Utilizing scripts and automation tools guarantees consistent setups and deployments, reducing human-induced errors.
  
- **Continuous Testing:** Rigorous testing at every stage of migration guarantees the functional integrity of the application, a critical aspect of the overall process.

---

In this MultiCloud migration journey, meticulous planning and adherence to best practices were paramount. By mastering the art of cloud migration, I have not only accomplished this project but also acquired valuable skills essential for any cloud computing professional.

Thank you for your time, and I am ready to answer any questions you might have regarding this hands-on project. Let's embrace the cloud future together! 🚀
