# ToCS_Project
This is the Final Project of Topics in Computer Science I .
# Blog Project

This is a simple blog project that includes the following pages:

- **signup.html**: Page for users to sign up for the blog.
- **login.html**: Page for users to log in to the blog.
- **index.html**: Main page with a list of blog posts (can be customized).
- **create.html**: Page for creating a new blog post.
- **view.html**: Page for viewing individual blog posts.
- **style.css**: Custom styles for the blog pages.

The project is deployed on an EC2 instance running Apache, and a Jenkins pipeline automates the deployment process.

## Project Setup

### Prerequisites

1. **Apache**: The project requires Apache to be installed and running on an EC2 instance.
2. **Jenkins**: Jenkins is used for automating the deployment of the project files to the Apache server.
3. **Git**: The GitHub repository should be accessible by Jenkins.
4. **SSH Access**: Jenkins should have SSH access to the EC2 Apache server to deploy files.

### Steps to Set Up the Project

1. **Clone the GitHub Repository**

   Clone the repository containing the blog project files to your local machine or server.

   ```bash
   git clone https://github.com/Sami-1166/Assignment4.git
