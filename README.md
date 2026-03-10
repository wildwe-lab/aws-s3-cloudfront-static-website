I created a static website using Amazon S3 and CloudFront.
First, I created the HTML page (index.html) and got the images I wanted from google  to display on the website.
Then I created an S3 bucket and kept the "Block all public access" setting enabled so that the content can only be accessed through CloudFront.
After that, I uploaded the website files (index.html and images) to the S3 bucket.
Next, I created a CloudFront distribution and selected the S3 bucket as the origin.
I configured Origin Access Control (OAC) to allow CloudFront to securely access the S3 bucket.
Then I added the required bucket policy to allow CloudFront to retrieve the objects from the bucket.
Finally, I set the default root object to index.html and deployed the distribution.
After the deployment was completed, I used the CloudFront domain name URL to access the website
