# Deployed-a-Static-Website-on-AWS-
Hosted and managed a web project using AWS services,  leveraging S3 for storage and Route 53 for domain management. It  ensured reliable website availability and performance.


**Set-Up Instructions**

Below are the steps to deploy static Website on Amazon S3. You can follow these instructions to deploy your own static Website.
Open AWS Management console. Select S3 under Storage.

# Step 1 - Create an S3 Bucket
    When you first create an S3 bucket, you select the AWS Region in which the files will be geographically stored.
    
    Click on "Create Bucket" button.
    
    Provide a globally unique name for bucket and select Region.

Leave blank this field "Copy Settings from an existing bucket".
# Step 2 - Upload Content of your Website
Upload the website contents to your S3 bucket including sub-folders.

For Example: You can use sample Website "Website" folder contents (provided in this repository).

NewLogin.html
error.html
NewLogin.css

# Step 3 - Add a Bucket Policy to allow Public Read Access
Go to Permissions Tab and update Public Access Setting:

Uncheck Manage public bucket policies:

**->** Uncheck - Block new public bucket policies (Recommended)

**->** Uncheck - Block public and cross-account access if bucket has public policies (Recommended)

# Step 4 - Enable Website Hosting

In order to serve assets via url, you need to enable Website Hosting

Go to Properties and enable "Static Website Hosting" option

Note the endpoint. http://{bucket-name}.s3-website-{AWS-Region}.amazonaws.com

# Step 5 - Access Your Website (Testing/Validation)
Access the site in browser: http://{bucket-name}.s3-website-{AWS-Region}.amazonaws.com

For Example: http://jayasuryapanduru1.click.s3-website.ap-south-1.amazonaws.com/


## Advantages of Hosting Website on S3
Here are some of the advantages of hosting site on S3

**Performance**: The website will be highly performant and scalable at a fraction of the cost of a traditional Web server.

**Scalability:** Amazon S3 is inherently scalable. For popular websites, the Amazon S3 architecture will scale seamlessly to serve thousands of 
                 HTTP requests per second without any changes to the architecture.

**Availability:** In addition, by hosting with Amazon S3, the website is inherently highly available.
