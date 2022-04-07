# Deploy-model-using-Flask-on-AWS

### Steps:
1. Built Amazon Fine Food reviews model and stored the model and other key model related variables in .pkl files
2. Launched a micro instance on AWS.
3. Connected to the AWS box [ssh]:
      ssh -i "my_key_pair.pem" ubuntu@ec2-65-0-6-52.ap-south-1.compute.amazonaws.com
4. Moved the files to AWS EC2 instance/box [scp]:
      scp -r -i "my_key_pair.pem" ./AFR ssh -i "my_key_pair.pem" ubuntu@ec2-65-0-6-52.ap-south-1.compute.amazonaws.com:~/
5. Installed all packages needed on the AWS box.
      Packages required: pip3, pandas, numpy, sklearn, beautifulsoup4, lxml, flask, re
6. Run python3 app.py on the AWS box.
7. Output in the browser.
      address: ipv4address:8080/index
