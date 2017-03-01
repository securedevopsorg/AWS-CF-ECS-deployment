# AWS exercise - Using CloudFormation to deploy a multi-Availability Zone Docker deployment with a two part web application (a product service and web service for formatting)

Goal: Deploy the infrastructure for a basic protected web application which runs in docker; by using CloudFormation templates.

Implement CD pipeline on AWS with Zero Downtime deploy of a single http service.

AWS Infrastructure components used:

* ECS (AWS Docker Container Service)
* VPC - Virtual Private Cloud infrastructure. One VPC is deployed per Availability Zone.
* ALB - Application Load Balancer. A special type of Load Balancer used to balance across web application deployments like those in this example. The instance 'checks in' with the ALB once it is completely running, which signals the ALB to begin sending application requests.
