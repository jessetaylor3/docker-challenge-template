# docker-challenge-template

**CHALLENGE ONE**
Step 1: Created index.html in challenge 1 folder to display my name and ID
Step 2: Created DockerFile outside of public folder.
Step 3: Use NGINX image from docker hub

FROM nginx: alpine

Step 4: Copy contends of public folder to the directory where Nginx serves its pages: 

COPY public /usr/share/nginx/html 

Step 5: Expose port 80

EXPOSE 80

Step 6: Start Nginx and keep it running in the foreground

CMD ["nginx", "-g", "daemon off;"]

Step 7: Navigate to folder directory in terminal
Step 8: Enter command to build docker image

    "docker build -t my-nginx-server ."

Step 9: Run image with following command:

    "docker run --name my-running-server -d -p 8080:80 my-nginx-server"

Step 10: Screenshot both running in docker and the site it serves
- Screenshots placed in folder directory and will also be submitted on d2l

**CHALLENGE 2**
