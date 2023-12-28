# Use the official Nginx base image
FROM nginx

# Copy custom Nginx configuration
#COPY nginx.conf /etc/nginx/nginx.conf

# Copy HTML files to the Nginx web server root
COPY ./html /usr/share/nginx/html

# Copy image files to a subdirectory in the Nginx web server root
COPY ./images /usr/share/nginx/html/images

# Expose port 80 to the outside world
EXPOSE 80

# Start Nginx when the container runs
CMD ["nginx", "-g", "daemon off;"]