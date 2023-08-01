# Containerized Load Balancer
Super simple Nginx load balancer in a container.

Replace `$SERVER_IP_X` in `nginx.conf` with the IPs of your servers.

Use the commands below to run the load balancer. Make sure to replace `$IMAGE_ID` with the ID of the image built by `docker build`. `docker images` will list all available images.

```text
sudo docker build .
sudo docker run -p 80:80 -d --restart always $IMAGE_ID
```
