<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Host a Website on Amazon S3

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-host-a-website-on-s3)

**Author:** francesj7837@gmail.com  
**Email:** francesj7837@gmail.com

---

![Image](http://learn.nextwork.org/easygoing_lavender_peaceful_durian/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Introducing Today's Project!

### What is Amazon S3

Amazon S3 is a storage space to upload website files and host them to cloud so that it can be known to public. This is useful because you have full control of who gets to access your bucket.

### How I used Amazon S3 in this project

I used it to learn how to create a bucket, upload web files and assets and host them to public.

### One thing I didn't expect in this project was...

The error message which I find it useful because I get to learn how to resolve the issue.

### This project took me...

It took me less than 30 mins!

---

## How I Set Up an S3 Bucket

Creating an S3 bucket took me less than 5 mins to create and have a good understanding of the entire set up. 

I picked Central Canada as the region because this is where I'm closest to.

S3 bucket names are globally unique this means no other buckets are named after the ones you picked, unless you deleted your own then someone can use it.

![Image](http://learn.nextwork.org/easygoing_lavender_peaceful_durian/uploads/aws-host-a-website-on-s3_ba6d42ad)

---

## Upload Website Files to S3

### index.html and image assets

I uploaded two files to my S3 bucket - they were  the index.html and a folder named NextWork - Everyone should be in a job they love_files/

Both files are necessary for this project as they contain the asset files that is needed for creating the website. 

![Image](http://learn.nextwork.org/easygoing_lavender_peaceful_durian/uploads/aws-host-a-website-on-s3_a265af88)

---

## Static Website Hosting on S3

Website hosting means to show my website to the public where anyone who knows about my web URL can view it in their device

To enable website hosting with my S3 bucket, ' have to go to Properties tab and select Static website hosting and enable it.

An ACL is managing who can access and what type of files to upload in my bucket.

![Image](http://learn.nextwork.org/easygoing_lavender_peaceful_durian/uploads/aws-host-a-website-on-s3_c22c54c0)

---

## Bucket Endpoints

Once static website is enabled, S3 produces a bucket endpoint URL, which is the link to my website

When I first visited the bucket endpoint URL, I saw the 403 error message. The reason for this error was that the objectst that I uploaded are not made for public yet so I have to take action and make them public.

![Image](http://learn.nextwork.org/easygoing_lavender_peaceful_durian/uploads/aws-host-a-website-on-s3_22ce4daf)

---

## Success!

To resolve this connection error, I have to go to Objects tab, select all the files I uploaded, go to Actions and select Make public using ACL. 

![Image](http://learn.nextwork.org/easygoing_lavender_peaceful_durian/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Bucket Policies

An Alternative to ACLs are bucket policies, which are conditions for managing files inside the bucket. The benefit of using bucket policies is I can control the objects available in the bucket while ACLs are useful for delete, change and more.

My bucket policy that I set the file named index.html not to be deleted was saved. I tested this by trying to delete the file and saw the message that says 'Failed to delete objects'. This means the policy that I created worked.

![Image](http://learn.nextwork.org/easygoing_lavender_peaceful_durian/uploads/aws-host-a-website-on-s3_sm2sm2sm)

---

---
