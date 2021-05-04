# py-flask-signup-docker
This Python sample application is based on the [eb-py-flask-signup](https://github.com/awslabs/eb-py-flask-signup) sample. It has been modified to run on Amazon EC2 Container Service (ECS) and use the ecs-cli.



# aws ecs create-service --cluster ECSNestedTraining --service-name flask-signup-service --task-definition flask-signup --load-balancers loadBalancerName=jenkins-demo,containerName=flask-signup,containerPort=5000 --role ecs-service-role --desired-count 0