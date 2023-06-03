# ecr-fargate-nodejs

```sh
# deploy commands
aws ecr get-login-password --region ap-northeast-1 | docker login --username AWS --password-stdin 860443256809.dkr.ecr.ap-northeast-1.amazonaws.com
docker build -t ecs-fargate-nodejs .
docker tag ecs-fargate-nodejs:latest 860443256809.dkr.ecr.ap-northeast-1.amazonaws.com/ecs-fargate-nodejs:latest
docker push 860443256809.dkr.ecr.ap-northeast-1.amazonaws.com/ecs-fargate-nodejs:latest
```
