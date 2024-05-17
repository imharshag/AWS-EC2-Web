# Hosting a Website Using MobaXterm in AWS - EC2

### Overview
🌐🛠️ Launching a server and hosting a website with Apache HTTP Server using MobaXterm involves several steps, including provisioning an Amazon EC2 instance, configuring the instance with Apache HTTP Server, and deploying the website files. MobaXterm facilitates remote access and management of the server, allowing users to execute commands, transfer files, and monitor the server's performance. This guide provides a step-by-step overview of the process.

### Preview of Website
Click here! to visit the website.

### Hosting a Website with Apache HTTP Server Using MobaXterm

***Step 1: Provisioning an Amazon EC2 Instance***
- Log in to the AWS Management Console and navigate to the EC2 dashboard.
- Click on the "Launch Instance" button to initiate the instance creation process.
- Choose an Amazon Machine Image (AMI), such as Amazon Linux, as the operating system for the instance.
- Select an instance type based on your requirements, ensuring sufficient CPU, memory, and storage resources.
- Configure instance details, including network settings, security groups, and key pairs for SSH access.
- Review and launch the instance, then select an existing key pair or create a new one for SSH access.
  
***Step 2: Connecting to the EC2 Instance with MobaXterm***
- Open MobaXterm and create a new SSH session by entering the public IP address or DNS name of the EC2 instance.
- Use the key pair generated during instance creation to authenticate the SSH session.
- Once connected, users can execute commands on the EC2 instance's terminal directly from MobaXterm's interface.

***Step 3: Installing and Configuring Apache HTTP Server***
- Update the package repository on the EC2 instance by running the command: sudo yum update -y.
- Install Apache HTTP Server using the command: sudo yum install httpd -y.
- Start the Apache service and enable it to start automatically on boot with the commands:
    - start service httpd

***Step 4: Deploying the Website Files***
- Transfer the website files to the EC2 instance using MobaXterm's SFTP feature or SCP command.
- Place the website files in the directory configured in Apache's configuration file, typically located at /var/www/html.
- Ensure that the website files have the correct permissions set to be accessible by Apache.

***Step 5: Accessing the Website***
- Open a web browser and enter the public IP address or DNS name of the EC2 instance.
- If configured correctly, the website hosted on Apache HTTP Server should be accessible and displayed in the browser.

### Contact Information
For inquiries or feedback, please contact **[Harsha G](mailto:harshag3106@gmail.com)**

### Contributing
🛠️ Contributions are welcome! Feel free to open an issue or submit a pull request with any improvements or bug fixes.
