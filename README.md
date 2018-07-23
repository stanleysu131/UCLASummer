# UCLASummer
SSH keys
- Using bash, create an SSH key: 'ssh-keygen'
Amazon EC 2
- On AWS, navigate to EC2 to launch a new instance or create a security group.
Security Groups
- Create a new security group indicating which inbound networks to allow.
AWS Operating System
- Select ubuntu as the AWS Operating System when launching instance.
Docker Installation
- In bash, connect to AWS operating system "ssh ubunto@'public IP address'"
- Install Docker with "curl -sSL https://git.docker.com | sh"
- "sudo usermod -aG docker ubuntu"
Obtaining the correct Docker image
- Use "docker pull ..." to obtain correct docker image 
- i.e "docker pull jupyter/datascience-notebook"
Running the correct Docker image as a container
- Use "docker run ..." to run docker image
- "docker run -d -p 443:8888 -v /home/ubuntu:/home/jovyan jupyter/datascience-notebook"
Jupyter notebook security concerns

A detailed budget of the costs of running a Jupyter Data Science Notebook Server for three months using at least three different kinds of EC 2 instances.
- m4.16xlarge; $3.20 per Hour;  2190 hours = $7,008 
- r4.16xlarge; $4.256 per Hour; 2190 hours = $9,320.64
- t2.micro;    $0.0116 per Hour;2190 hours = $25.404

