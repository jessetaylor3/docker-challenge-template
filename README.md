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

Step 1: Use the challenge2 folder, already containing package-lock.json, package.json, and server.js for our simple NodeJS application.
Step 2: Create a Dockerfile in the challenge2 directory to build our NodeJS application's Docker container.
Step 3: Created a docker-compose.yml file in the same directory to orchestrate the web server and the application.
Step 4: Created an nginx.conf file for Nginx to listen on port 8000 and forward requests to the NodeJS application.
Step 5: Navigated to the challenge2 directory in the terminal.
Step 6: Entered the command to build and run the Docker containers:

    "docker-compose up --build"

Step 7: After confirming all services were running properly, open a browser and pointed it to "http://localhost:8000/api/books" to see a JSON message with all books.
Step 8: Screenshots of the running server in Docker, the page being served (http://localhost:8000/api/books), and the Docker Compose logs were taken.