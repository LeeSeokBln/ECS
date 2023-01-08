# ECS-Port-range
```
32768 - 65535
```
# taskdef.json
```
{
 "executionRoleArn": "arn:aws:iam::[ACCOUNT-ID]:role/ecsTaskExecutionRole",
 "containerDefinitions": [{
  "name": "[CONTAINER-NAME]",
  "image": "<IMAGE>",
  "essential": "true",
  "portMappings": [{
    "protocol": "tcp",
    "containerPort": [CONTAINER-PORT]
  }]
 }],
 "requiresCompatibilitiess": [
   "EC2"
 ],
 "cpu": "512",
 "memory": "512",
 "family": "[TASK-NAME]"
}
```
