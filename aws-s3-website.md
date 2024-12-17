---
layout: default
title: "AWS S3 Website with CloudFront"
permalink: /aws-s3-website/
---

# 🚀 AWS S3 Website with CloudFront

<!-- LinkedIn logo and link at the top -->
<div style="text-align: center; margin-bottom: 20px;">
  <a href="https://www.linkedin.com/in/cameron-ws/" target="_blank" aria-label="LinkedIn">
    <img src="https://cdn-icons-png.flaticon.com/512/61/61109.png" alt="LinkedIn" style="width: 30px; height: 30px;"/>
  </a>
</div>


# AWS S3 Website with CloudFront

This project demonstrates hosting a secure, cost-effective static website using AWS S3 and CloudFront.

---

## 🚀 Project Overview

- **Purpose**: Deploy a static website securely with global content delivery.
- **Technologies**:
  - **AWS S3**: Storage and static hosting.
  - **CloudFront**: Global CDN for performance and HTTPS.
  - **IAM**: Secure role-based access.

---

## 🛠️ Architecture

The setup includes:
- An **S3 bucket** for static file storage.
- A **CloudFront distribution** for HTTPS access and global delivery.
- IAM role for secure S3 access.

![Architecture Diagram1](/images/aws-s3-web-diagram)
![Architecture Diagram2](aws-s3-web-diagram)
![Architecture Diagram3](/images/aws-s3-web-diagram.png)
![Architecture Diagram4](/aws-s3-web-diagram)

---

## 🔧 Step-by-Step Setup

### 1. S3 Bucket Configuration
- Enable **Static Website Hosting**.
- Upload `index.html` and `error.html`.

### 2. CloudFront Distribution
- Connect CloudFront to the S3 bucket.
- Enable HTTPS and configure caching.

### 3. Security Hardening
- Block direct public access to S3.
- Use **Bucket Policies** and **Origin Access Identity**.

---

## 🖥️ Testing the Setup

1. Visit the CloudFront domain.
2. Verify:
   - The home page (`index.html`) loads.
   - Error handling works (`error.html`).

---

## 💡 Key Learnings

- Configuring static website hosting with S3.
- Enhancing security with IAM roles and CloudFront.

---

## 🔒 Security Best Practices

- **HTTPS**: Enforced via CloudFront.
- **S3 Block Public Access**: Ensures no direct file access.
- **IAM Policies**: Fine-grained access control.

---

## 📜 Code and Resources

- **Bucket Policy**: [bucket-policy.json](bucket-policy.json)
- **Sample HTML**:
  - `index.html`
  - `error.html`

---

## 📝 Future Improvements

- Integrate Route 53 for custom domains.
- Implement CloudWatch for monitoring and logging.




---

