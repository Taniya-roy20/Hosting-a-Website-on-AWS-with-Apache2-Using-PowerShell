# Hosting a Website on AWS with Apache2 Using PowerShell
**(These are the steps after launching instance and downloading .pem passkey)**
<br>
Step 1: Connect to EC2 Instance Using PowerShell
Open PowerShell in Windows.
Navigate to your PEM file: First, ensure you’re in the directory where your .pem file is located. Use cd to change directories:
cd path\to\your-pem-file
Use the ssh command to connect to your EC2 instance:
ssh -i "your_key.pem" ec2-user@your_instance_public_IP
Replace path_to_your_key.pem with the location of your private key. Replace your_instance_public_IP with the public IP of your EC2 instance.
