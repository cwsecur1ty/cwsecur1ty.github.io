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

This project demonstrates hosting a secure, cost-effective static website using AWS S3 and CloudFront.

---

## AWS S3 - Overview

- **Purpose**: Deploy a static website securely with global content delivery.
- **Technologies**:
  - **AWS S3**: Storage and static hosting.
  - **CloudFront**: Global CDN for performance and HTTPS.
  - **IAM**: Secure role-based access.

---

## Architecture & Lucid Chart

Setup includes:
- An **S3 bucket** for file storage.
- A **CloudFront distribution** for HTTPS access and global delivery.
- IAM role for secure S3 access.

![Architecture Diagram](/images/aws-s3-web-diagram)

---

## Step-by-Step Setup & Configuration (S3 Bucket & Web)

### 1. Create the S3 Bucket on AWS
- Log in to the AWS Management Console.
- Click Create Bucket
  - Name the bucket something great like: 'camerons-epic-s3'
  - Disable "Block all public access" (temporarily for setup)
- Scroll down and click '**Create bucket**'

### 2. Enable Static Website Hosting on S3
- Navigate to the Bucket.
- Enter the properties page.
- Scroll down to 'Static website hosting' (this is at the bottom).
  - Click 'Edit'
  - Change from 'Disable' to 'Enable' (**At this point I needed to create an index.html & error.html to host on the Bucket - you will too.**)
- For now, just name the two files, I kept it simple with index.html & error.html.

### 3. Upload Web Content to the S3
- Navigate back to the Overview page.
- Click 'Upload' and upload your index.html & error.html.

### 4. Configure CloudFront for Content Delivery
- Navigate to CloudFront (I did this by the very top search bar and searching 'CloudF'
- Click Create Distribution.
- Follow this:
  - Set the Origin Domain to your s3. (Mine is: camerons-epic-s3)
  - Change Origin Access to OAC (This superseded OAI)
  - Click 'Create new OAC' & name it.
  - Under 'Default cache behaviour' use the default policy.
  - In Default Cache Behavior:
    - Viewer Protocol Policy: Redirect HTTP to HTTPS.
    - Allowed HTTP Methods: GET, HEAD (for static content).
  - Under 'Default Root Object' set this to
    - index.html
- Finally, click 'Create Distribution'

### 5. Update the S3 Bucket Policy for OAC
- On the page of your newly created CloudFront there should be a yellow warning regarding your OAC policy.
- Follow these steps:
  - Click 'Copy policy'.
  - Navigate to the S3 console.
  - Select your bucket.
  - Go to the Permissions tab.
  - Scroll down to the 'Bucket policy' section & click 'Edit'
  - Paste the copied policy into the editor.
  - Click 'Save Changes'.

### 6. Verify
- Go back to the **CloudFront Console**.
- Open up your Distribution.
- Verify the warning is no longer present.
- Test your domain URL which in my case is: [Here](https://d1l9lyx1eakae6.cloudfront.net)

---

## Key Learnings

- Configuring static website hosting with S3.
- Enhancing security with IAM roles and CloudFront.

---

## 🔒 Security Best Practices

- **HTTPS**: Enforced via CloudFront.
- **S3 Block Public Access**: Ensures no direct file access.
- **IAM Policies**: Fine-grained access control.

---

## 📝 Future Improvements

- Integrate Route 53 for custom domains.
- Implement CloudWatch for monitoring and logging.



---

