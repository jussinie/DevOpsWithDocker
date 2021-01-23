This is a simple build service. It will pull a repo from Github, create a Docker image from it and push it to Docker Hub.  
**Requirements:**  
Github repo needs to have a Dockerfile. 
You will also need to have an account in Docker hub. 
The service will prompt you to give the url to the github repo. 
After that you need to give a folder name (that is the last part from the github repo name) 
In the end, provide your docker username and password. 
  
**How to use**  
Download files to your local folder.  
Build by using: docker build . -t image_name_you_want  
Run with: docker run -it -v /var/run/docker.sock:/var/run/docker.sock image_name_you_want
