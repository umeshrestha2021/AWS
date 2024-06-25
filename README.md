# AWS
# File user-data
#step1
1. On the top navigation bar, review the Region selector to ensure that the Region is set to N. Virginia (us-east-1).
2. In the Services search box, type:
ec2
3. In the search results, under Services, click EC2.
4. Go to the next step.
#Step2
1. In the left navigation pane, click EC2 Dashboard.
2. In the Launch instance section, click Launch instance.
3. Go to the next step.
#Step3
1. In the Name and tags section, for Name, type a name that you like, such as: webserver01.
2. In the Application and OS images section, under Quick Start, choose Amazon Linux.
3. Scroll down to Amazon Machine Image (AMI).
4. Go to the next step.
#Step4
1. Click the Amazon Machine Image (AMI) dropdown menu.
2. Choose Amazon Linux 2 AMI (HVM).
- Be sure to choose Amazon Linux 2, not Amazon Linux 2023 AMI, or your launch will fail.
3. For Instance type, if not already selected, choose t2.micro.
4. Scroll down to Key pair (login).
5. Go to the next step.
#Step6
1. For Key pair name, choose Proceed without a key pair. 
2. In the Network settings section, click Edit.
3. Go to the next step.
#Step7
1. For VPC, choose LabVpc.

- Your solution will fail if you do not choose this VPC.

2. For Subnet, choose the subnet in the us-east-1a Availability Zone.

- Note the AZ choices on the dropdown list. In the later DIY section of this solution, you must choose the subnet in the other AZ.

3. Go to the next step.
#Step8
1. For Security group name, type: 

Security-Group-Lab

2. For Description, type: 

HTTP Security Group

3. For Type, choose HTTP.
4. Scroll down to Configure storage.
5. Go to the next step.
Step9
1. In the Configure storage section, for Root volume, choose gp2 from the dropdown menu. 

- If gp3 is selected, confirm that you chose the correct AMI in a previous step.

2. Click to expand the Advanced details section.
3. Go to the next step.
Step10
1. Open the user-data file that you downloaded earlier, and then review the content.

- This user data script launches a web server, using port 80, to display internal information about the instance.
- The code block in your file is longer than what is displayed in the screenshot example.

2. Go to the next step.
Step11
1. On the console, scroll down to User data.
2. Click Choose file.
3. Select the user-data file that you review in previous step (not shown).
4. Go to the next step.
Step12
1. Review the User data content.
2. Go to the next step.
Step13
1. Review the Summary section.  

- The Summary section, when your browser is fully expanded, will float on the right side. 

- For Software Image (AMI) confirm you have selected Amazon Linux 2.

2. Click Launch instance.
3. Go to the next step.
Step14
1. In the success alert, review the message.
2. Scroll down to the bottom of the page.
3. Go to the next step.
Step15
1. Click View all instances.

- If you receive an error related to insufficient capacity, try using the t3 instance family instead of t2.

2. Go to the next step.
Step16
1. In the Instances section, choose the check box to select your EC2 instance.
2. Under Instance state, review to ensure that the instance is Running before proceeding.
3. After the instance state displays Running, under Public IPv4 DNS, click the copy icon to copy the provided address.

- Do not use the "open address" link.

4. Go to the next step.
