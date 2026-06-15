# Task 2 - Set Up a Static Website on AWS S3

## Objective

Host a static website using Amazon S3 Static Website Hosting.

## Tools Used

* Amazon S3
* AWS Management Console
* HTML

## Bucket Details

* Bucket Name: rd-infro-task2-nikhil-2026
* Region: Europe (Stockholm) - eu-north-1

## Steps Performed

1. Logged in to the AWS Management Console.
2. Opened Amazon S3 service.
3. Created a new S3 bucket named **rd-infro-task2-nikhil-2026**.
4. Disabled Block Public Access settings.
5. Uploaded the website file (**index.html**) to the bucket.
6. Enabled Static Website Hosting in bucket properties.
7. Configured **index.html** as the index document.
8. Added a bucket policy to allow public read access.
9. Accessed the website through the S3 Website Endpoint.
10. Verified successful website hosting.

## Bucket Policy Used

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicRead",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::rd-infro-task2-nikhil-2026/*"
    }
  ]
}
```

## Website Files

### index.html

```html
<!DOCTYPE html>
<html>
<head>
    <title>RD INFRO TECHNOLOGY Internship</title>
</head>
<body>
    <h1>Welcome to My AWS S3 Static Website</h1>
    <h2>Created by Nikhil</h2>
    <p>Task 2 - Static Website Hosting using AWS S3</p>
</body>
</html>
```

## Screenshots Included

1. S3 Bucket Created
2. index.html Uploaded
3. Static Website Hosting Enabled
4. Bucket Policy Configuration
5. Website Running in Browser

## Result

Successfully hosted a static website using Amazon S3 Static Website Hosting. The website was made publicly accessible through the S3 website endpoint by configuring bucket permissions and enabling static website hosting.
