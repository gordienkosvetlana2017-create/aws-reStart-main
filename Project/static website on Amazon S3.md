Configuring a Static Website on Amazon S3 Project Overview This project was completed as a group assignment for four people to create a static restaurant website hosted on Amazon S3.We developed a website for a keto-kitchen restaurant named KetoLife Café.The project requirements included displaying the restaurant name, a description, at least five menu items, and contact information.The site features the story of four women—Dipti, Svetlana, Valerie, and Zineb—who started the restaurant in Zurich.We used AI prompts to generate the HTML files and images, creating specific sections for "About Us," "Keto Menu," and "Contact Us".Technical Implementation 1. Bucket Configuration We created an S3 bucket named keto-life-cafe in the us-west-2 (Oregon) region.2. Static Website Hosting Static website hosting was enabled via the Properties tab.The Index document was set to index.html.The Error document was set to error.html.3. Permissions and Public Access We disabled the Block all public access setting to allow external access to the site.A Bucket Policy was applied to grant s3:GetObject permissions to all users.JSON{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "PublicReadGetObject",
            "Effect": "Allow",
            "Principal": "*",
            "Action": "s3:GetObject",
            "Resource": "arn:aws:s3:::keto-life-cafe/*"
        }
    ]
}
Troubleshooting Initially, the site returned a 404 Not Found error.This happened because the files were uploaded inside a folder named static-website 2/ instead of the bucket root.After moving the objects to the root directory, the website became fully functional.Final Result The KetoLife Café website is now live and accessible through the S3 website endpoint.
