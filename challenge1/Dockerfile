# Use the Nginx image from Docker Hub
FROM nginx:alpine

# Copy the contents of the public folder to the directory where Nginx serves its pages
COPY public /usr/share/nginx/html

# Expose port 80 to the outside world
EXPOSE 80

# Start Nginx and keep it running in the foreground
CMD ["nginx", "-g", "daemon off;"]
