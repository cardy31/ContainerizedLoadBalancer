# Containerized Load Balancer
Super simple Nginx load balancer in a container.

Commands to run it. Make sure to replace `$IMAGE_ID` with the ID of the image built by `docker build`.

```text
sudo docker build .
sudo docker run -p 80:80 -d --restart always $IMAGE_ID
```
