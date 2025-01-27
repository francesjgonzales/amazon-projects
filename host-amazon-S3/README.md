# Host a Website on Amazon S3

A guide to hosting a static website using Amazon S3. This project demonstrates the steps and key learnings from hosting a website on AWS S3.

---

## What is Amazon S3?

Amazon S3 is a cloud storage service where you can:

- Upload website files.
- Host them publicly for access via a URL.
- Control access to your bucket.

**Why is it useful?**  
You have full control over access permissions and can manage your website's public availability.

---

## Project Overview

**What I Did:**

- Created an S3 bucket.
- Uploaded web files and assets.
- Enabled public hosting for the bucket.

**Unexpected Challenges:**  
Encountering a 403 error message when accessing the website, which was resolved by making the uploaded files public.

**Time Taken:**  
Less than 30 minutes!

---

## Step-by-Step Instructions

### 1. Setting Up an S3 Bucket

- Creating an S3 bucket takes less than 5 minutes.
- I selected "Central Canada" as the region for proximity.
- Bucket names must be globally unique.

### 2. Upload Website Files

Uploaded the following files to the S3 bucket:

- `index.html`
- `NextWork - Everyone should be in a job they love_files/`

### 3. Enable Static Website Hosting

- Navigate to the **Properties** tab in S3.
- Enable **Static website hosting**.
- An **Access Control List (ACL)** was used to manage file access.

### 4. Resolving 403 Error

- Initially, accessing the bucket endpoint URL resulted in a 403 error.
- Resolved by:
  - Going to the **Objects** tab.
  - Selecting all uploaded files.
  - Making them public using ACL.

### 5. Bucket Policies

- Configured a bucket policy to prevent deletion of `index.html`.
- Tested by attempting to delete the
