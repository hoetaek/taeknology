`sudo yum install -y docker`
https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/install-docker.html

## docker compose
```bash
sudo mkdir -p /usr/local/lib/docker/cli-plugins/
sudo curl -SL "https://github.com/docker/compose/releases/latest/download/docker-compose-linux-$(uname -m)" -o /usr/local/lib/docker/cli-plugins/docker-compose
sudo chmod +x /usr/local/lib/docker/cli-plugins/docker-compose
```
