# Use official Nginx image
FROM nginx:alpine

# Remove the default nginx website
RUN rm -rf /usr/share/nginx/html/*

# Copy your HTML and SVG files into Nginx's default directory
COPY . /usr/share/nginx/html

# Expose port 80 (standard HTTP)
EXPOSE 80

# Start Nginx in the foreground
CMD ["nginx", "-g", "daemon off;"]
