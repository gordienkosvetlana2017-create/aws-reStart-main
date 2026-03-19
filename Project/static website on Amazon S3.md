# Configuring a Static Website on Amazon S3.

## Project Overview 
This project was completed as a group assignment for four people to create a static restaurant website hosted on Amazon S3.
We developed a website for a keto-kitchen restaurant named KetoLife Café in Sandbox.
The project requirements included displaying the restaurant name, a description, at least five menu items, and contact information.

The site features the story of four women—Dipti, Svetlana, Valerie, and Zineb—who started the restaurant in Zurich.
We used AI prompts to generate the HTML files and images, creating specific sections for "About Us," "Keto Menu," and "Contact Us".

## Technical Implementation 
### 1. Bucket Configuration
 I created an S3 bucket named keto-life-cafe in the us-west-2 (Oregon) region.
 
<img width="500" height="324" alt="image4" src="https://github.com/user-attachments/assets/347d2d62-a8c8-4768-8803-865f7e6577a0" />

<img width="500" height="324" alt="image11" src="https://github.com/user-attachments/assets/32f64527-a8c4-4f34-8fd7-8df4413727da" />

  
### 2. Static Website Hosting
I enabled Static website hosting via the Properties tab. I set The Index document to index.html and the Error document to error.html.

<img width="500" height="324" alt="image2" src="https://github.com/user-attachments/assets/e86e8980-d3de-47b2-b22e-916d55463de2" />

   
### 3. Permissions and Public Access
   I disabled the Block all public access setting to allow external access to the site.
   
   <img width="500" height="324" alt="image7" src="https://github.com/user-attachments/assets/75cf8c7e-cdb3-4f57-9df6-b18dc3883e8d" />

   I applied a Bucket Policy to grant s3:GetObject permissions to all users:

<img width="500" height="324" alt="image10" src="https://github.com/user-attachments/assets/305e5e72-1d76-4de1-bc07-d85a650d5676" />

I checked website, it was not working.

<img width="500" height="324" alt="image1" src="https://github.com/user-attachments/assets/90197b39-a8fa-464c-8a07-74508fd45d49" />

<img width="500" height="324" alt="image3" src="https://github.com/user-attachments/assets/58358797-48f7-41a8-bacc-662c186ac03f" />

### 4. Troubleshooting 

Initially, the site returned a 404 Not Found error. This happened because the files were not uploaded on site. 

<img width="500" height="324" alt="image8" src="https://github.com/user-attachments/assets/a7502c34-e5ee-4ac6-afbf-06cd4e4a2ec9" />

I added the objects to the root directory, the website became fully functional.

<img width="500" height="324" alt="image6" src="https://github.com/user-attachments/assets/41c50e39-105a-4d45-8946-e6dbd6b4dc1d" />

Final Result The KetoLife Café website is now live and accessible through the S3 website endpoint.

<img width="500" height="324" alt="image5" src="https://github.com/user-attachments/assets/0243d302-82dd-4676-8a85-3f5908c17094" />

<img width="500" height="324" alt="Screenshot 2026-03-18 at 14 52 06" src="https://github.com/user-attachments/assets/3caf5486-b404-416b-bfc6-dbaf01337cca" />

<img width="500" height="324" alt="Screenshot 2026-03-18 at 14 52 10" src="https://github.com/user-attachments/assets/27620157-6ac9-421b-a080-bef3a87268d7" />

<img width="500" height="324" alt="Screenshot 2026-03-18 at 14 52 15" src="https://github.com/user-attachments/assets/7f7b82ee-96a1-4ccc-a81a-c68a64facd0d" />

<img width="500" height="324" alt="Screenshot 2026-03-18 at 14 52 19" src="https://github.com/user-attachments/assets/696f4cf6-a396-45a0-a31d-4a868d936eff" />
