# Static-website
Simple Static Website Hosting on S3

This is a simple static website hosted on **Amazon S3**, showcasing how to deploy a fully public, static website using AWS services.

## 🚀 Live Demo

👉 [Visit Live Site](http://sushma-portfolio-site.s3-website-us-east-1.amazonaws.com)

---

## 🧰 Tech Stack

- HTML5 
- AWS S3 (Static Website Hosting)
- S3 Bucket Policy for Public Access

---

## 🛠️ How I Deployed It

1. Created an S3 bucket with static website hosting enabled.
2. Uploaded HTML files using AWS Console.
3. Updated bucket policy to allow public access.
4. Tested using the public S3 endpoint.

---

## 📝 Bucket Policy Example

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadGetObject",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::sushma-portfolio-site/*"
    }
  ]
}
