# Wrapmate ComfyUI. 


This repo includes files to run the docker container with ComfyUI on the AWS EC2 machine. 

### What's is ComfyUI ? 

**Comfy UI** - is a powerful tool which help us to run the Stable Diffusion model, and customize it by adding custom models


### Deploy to AWS EC2. Step by step 

1. Update yum
 
       bash  sudo yum update -y

2. Install docker

       sudo amazon-linux-extras install docker

3. Install docker compose tool

        sudo curl -L https://github.com/docker/compose/releases/latest/download/docker-compose-$(uname -s)-$(uname -m) -o /usr/local/bin/docker-compose

        sudo chmod +x /usr/local/bin/docker-compose

4. Start the docker
   

       sudo service docker start

5. Create a comfyui directory.

        mkdir comfyui
       

6. Clone this repo

        git clone https://github.com/blypa-maker/ComfyUI comfyui

7. Navigate to directory

         cd comfyui

8. Run app

         docker compose up

   
