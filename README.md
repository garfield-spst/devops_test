# Clone this repo to local and run npm install and npm start to check app locally is running or not.
# Create Docker file at root path of the repo, use nodejs base image.
# create docker compose file to create app service and mongodb service, don't worry about mongodb image docker will handle itself just describe mongodb as service in docker compose file.
# Create AWS free tier account, and launch t3.micro instance 
# go to ECR in AWS create a repository
# go to IAM create an user "devops_test", and select policies option and then select all options.
# now select IAM/Users/devop_test and copy aws_key_id and aws_secret_key and go to your github repo and select setting and then go to security and add these secrets.
# now go to EC2 instance copy public IP of the server, then go to security in github and create another secret "server_public_ip" and enter the EC2 instance ip.
# finally create deploy.yml at .github/workflows 
# after pushing the changes github action will automatically trigger the deployment to EC2 instance.
