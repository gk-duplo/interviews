# Practical Exercises

## Exercise 1: AWS and Terraform

### Objective

Demonstrate your ability to work with AWS and Terraform by completing the following tasks:

### Network Segmentation: Segment your network in AWS

**Tasks:**
1. Create a VPC.
2. Define and configure Subnets.
3. Set appropriate CIDR blocks.

### Internet Access: Enable internet access for your VPC resources

**Tasks:**
1. Set up an Internet Gateway (IGW).
2. Configure Route Tables to ensure internet access.

### EC2 Configuration: Launch and configure EC2 instances

**Tasks:**
1. Launch EC2 instances within the created VPC.
2. Configure instance settings as required.

### Security Management: Manage inbound and outbound traffic

**Tasks:**
1. Create and configure Security Groups to control traffic.

### Object Storage: Create and manage an S3 bucket

**Tasks:**
1. Set up an S3 bucket.
2. Define relevant permissions and policies.

### Web Server Installation and Load Balancing: Install a web server and set up a load balancer

**Tasks:**
1. Install a web server (e.g., Apache or Nginx) on an EC2 instance.
2. Create and configure a Load Balancer to distribute traffic.

---

## # Docker Exercise: Custom Nginx Web Server

## Objective

Create a Dockerfile to set up an Nginx web server based on an Ubuntu image, which serves a sample HTML file. Set up a CI/CD pipeline to automate the build and deployment of the Docker image.

## Instructions

### 1. Clone the Repository

- Fork the provided GitHub repository that contains a sample `index.html` file to your local machine.
- Repo: https://github.com/gk-duplo/docker.git

### 2. Create a Dockerfile

- Write a Dockerfile that:
  - Uses an official Ubuntu image as the base image.
  - Installs Nginx on the Ubuntu image.
  - Copies the `index.html` file into the Nginx directory where it will be served `/var/www/html/`. 
  - Sets the entrypoint to start Nginx when the container runs. `nginx -g daemon off`

### 3. Test the Docker Image

- Run the Docker container to ensure that Nginx serves the `index.html` file. Verify that the file is served correctly by opening your web browser and navigating to `http://localhost:80`.

### 4. Commit Your Changes

- Add the Dockerfile and `index.html` to your GitHub repository.
- Commit your changes and push them to the repository.

### 5. Set Up CI/CD Pipeline

- Create a CI/CD pipeline using GitHub Actions or Jenkins:
  - Configure it to build the Docker image from your repository.
  - Set it up to push the Docker image to a container registry such as Dockerhub or ECR.

## Submission Guidelines

- Ensure that your Dockerfile and `index.html` are committed to your GitHub repository.
- Verify that your CI/CD pipeline builds and pushes the Docker image successfully.
- Provide a link to your repository and any instructions needed to demonstrate that your setup works.

If you need an example of how to set up your Dockerfile or CI/CD pipeline, refer to the documentation for Docker and the respective CI/CD tools you are using.

---

Good luck with the exercise!

