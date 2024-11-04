# Hosting a Website on AWS with Apache2 Using PowerShell
**(These are the steps after launching instance and downloading .pem passkey)**
<br>
**Step 1: Connect to EC2 Instance Using PowerShell**
<br>
1.Open PowerShell in Windows.
<br>
2.Navigate to your PEM file: First, ensure you’re in the directory where your .pem file is located. Use cd to change directories:

        cd path\to\your-pem-file
3.Use the ssh command to connect to your EC2 instance:

       ssh -i "your_key.pem" ec2-user@your_instance_public_IP
Replace path_to_your_key.pem with the location of your private key. Replace your_instance_public_IP with the public IP of your EC2 instance.
<br>
<br>
**Step 2: Update the Package List on Your EC2 Instance**
<br>
Run the following command after logging in to update your packages:

     sudo apt update
**Step 3: Install Apache2**
<br>
To install the Apache2 web server:

     sudo apt install apache2 -y
**Step 4: Delete the Default index.html and Create Your Own**
Navigate to the Apache web directory:

      cd /var/www/html
1.Delete the default index.html file:

      sudo rm index.html
2.Create a new index.html file:
   
      sudo vi index.html
**Add your website's HTML content and save the file.**
<br>
<br>
**Your link or IP adress of your instance will now work.**
