# Host a Website on Amazon S3

## Introduction
This project demonstrates how to host a static website using **Amazon S3**. Amazon S3 (Simple Storage Service) allows users to store and retrieve data, including website files, in highly scalable storage buckets.

## Project Details
- **Author:** P. Amaravathi
- **Platform:** [NextWork.org](https://community.nextwork.org/c/i-have-a-question?automatic_login=true)
- **Estimated Completion Time:** 15 minutes

## What is Amazon S3?
Amazon S3 is a storage service where each **S3 bucket name is globally unique**. Once a bucket is created, no other AWS account can use that name unless the bucket is deleted.

## Steps to Host a Website on S3

### 1. Create an S3 Bucket
- Creating a bucket takes less than **2 minutes**.
- **Selected Region:** `US East (N. Virginia) us-east-1`.
- Ensure that the **bucket name is globally unique**.
- ![Amazon S3 Setup](https://your-bucket-name.s3.amazonaws.com/s3-setup.png)


### 2. Upload Website Files
- Upload `index.html` and necessary image assets.
- These files are essential for setting up the website.
- ![Amazon S3 Setup](https://your-bucket-name.s3.amazonaws.com/s3-setup.png)

### 3. Enable Static Website Hosting
To enable public access to the website:
- Go to the **S3 bucket settings** and choose `Enable` for **Static Website Hosting**.
- Select `Host a static website` as the hosting type.
- Set `index.html` as the **Index Document**.
- Modify the **ACL (Access Control List)** to allow public access.
- ![Amazon S3 Setup](https://your-bucket-name.s3.amazonaws.com/s3-setup.png)

### 4. Bucket Endpoint & Public Access
- Once static website hosting is enabled, AWS provides a **Bucket Endpoint URL**.
- Initially, visiting the URL may result in a **403 Forbidden Error** due to private object permissions.
- To fix this:
  - Select `index.html` and the asset files.
  - Click **Actions** → `Make public using ACL`.
  - ![Amazon S3 Setup](https://your-bucket-name.s3.amazonaws.com/s3-setup.png)

### 5. Success!
- After adjusting the permissions, the static website will be publicly accessible.
- The project successfully demonstrates hosting a website on Amazon S3.
- ![Amazon S3 Setup](https://your-bucket-name.s3.amazonaws.com/s3-setup.png)

## Additional Resources
For more projects and community discussions, visit:
[NextWork.org](https://community.nextwork.org/c/i-have-a-question?automatic_login=true)
