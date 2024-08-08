# S3-STatic-Web-Hosting
## Hosting Static Website using AWS S3 Service 

Hosting a Static Website on AWS S3
This documentation guides you through hosting a static website on Amazon Simple Storage Service (S3). S3 is a scalable and cost-effective object storage service that can be used to host static websites.
Prerequisites:
•	An AWS account with appropriate permissions to create S3 buckets and modify bucket settings.
Steps:
## 1.	Create an S3 Bucket:
	Open the AWS Management Console and navigate to the S3 service https://console.aws.amazon.com/s3/.
o	Click on "Create bucket".
o	Choose a unique name for your bucket (ideally matching your domain name) and select the desired region where you want to store your website's files.
o	Under "Permissions", keep the default settings for now (you can adjust access controls later). Click "Create bucket".
## ![image](https://github.com/user-attachments/assets/2fce2b57-7446-4898-9cf0-5d4283548db9)
## ![image](https://github.com/user-attachments/assets/9fc6daac-dfee-456a-af28-3c3854d0aa2e)


## 2.	Upload Your Website Files:
    In the S3 console, navigate to your newly created bucket.
    Click the "Upload" button. You can either drag and drop your website files (HTML, CSS, JavaScript, images, etc.) or choose "Add Files" to select them from your local machine.
 
## 3.	Enable Static Website Hosting:
In the bucket properties, locate the "Static website hosting" section.
o	Click "Edit".
o	Select "Use this bucket to host a website".
o	Enter "index.html" as the "Index document" (the file S3 will serve when a user requests the root of your website).
o	Click "Save".
## ![image](https://github.com/user-attachments/assets/740ef596-676e-4012-8546-e7c06acd923e)
 
## 4.	Set Up Public Access 
By default, objects in your S3 bucket are private. To make your website publicly accessible, you need to adjust the bucket's access control list (ACL).
o	In the bucket properties, go to the "Permissions" tab.
o	Under "Public access", click "Edit".
o	Select "Block all public access" (if you don't intend for anyone to access objects directly from the bucket) or "Yes, Grant public read access to all objects in this bucket" (if all objects should be publicly accessible).
o	Click "Save".
## ![image](https://github.com/user-attachments/assets/7de1c945-e63d-4d4d-b4c7-2ecc5a3fe475)
 
## Testing Your Website:
Once you've completed the steps above, you should be able to access your website by visiting the following URL:
https://aws-buk-for-web-hosting.s3.amazonaws.com/index.html
## ![image](https://github.com/user-attachments/assets/d11568e5-e6da-414f-851e-229f71119dc1)
