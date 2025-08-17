🚀 Dockerized Web App with AWS S3 + Elastic Beanstalk

The workflow:
1.	Built a custom Docker image locally that serves a static webpage using Nginx.
2.	Packaged the Dockerfile and index.html into a ZIP file.
3.	Uploaded the ZIP file to AWS S3, where Elastic Beanstalk automatically stored the deployment package.
4.	Deployed the app via Elastic Beanstalk, which pulled the code from S3, created an environment, and ran the Docker container on EC2.

🐳 Features
1.	Custom Docker image with Nginx serving static content.
2.	Local Docker testing before deployment.
3.	AWS S3 as deployment storage: all uploaded bundles automatically stored in an Elastic Beanstalk–created S3 bucket.
4.	Elastic Beanstalk environment: handled EC2 provisioning, scaling, and running the container.
5.	Publicly accessible web app hosted in the cloud.

⚙️ Tech Stack
1.	Docker – containerization platform
2.	Nginx – web server for static HTML
3.	AWS S3 – storage for deployment ZIPs
4.	AWS Elastic Beanstalk – automated app deployment and scaling
5.	AWS IAM – identity and access management

🛠️ Steps Completed
1.	Installed Docker Desktop and verified installation.
2.	Tested a sample Nginx container with:
  	  docker run -d -p 80:80 nginx
3.	Created a Dockerfile to serve a custom index.html.
4.	Built the image:
      docker build -t my-web-app .
5.	Ran and tested the image locally.
6.	Created a ZIP file (Dockerfile + index.html).
7.	Deployed via Elastic Beanstalk, which:
8.	Uploaded the ZIP to S3 automatically.
9.	Created an EC2 instance and ran the Docker container.
10.	Verified deployment via the Elastic Beanstalk domain.
11.	Deleted S3 bucket and Elastic Beanstalk environment to avoid charges.

🎉 Learnings
1.	Gained hands-on experience with Docker and Nginx.
2.	Understood how Elastic Beanstalk uses S3 for deployment storage.
3.	Practiced deploying a containerized app to the cloud with minimal manual setup.
4.	Learned how to manage and clean up AWS resources to avoid charges.
