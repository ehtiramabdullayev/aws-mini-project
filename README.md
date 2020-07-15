# aws-mini-project

Create mini public API which can do the basic CRUD operations on an entity (its your choice - it can be Cars, Hotels, Clothes, Books, Projects, etc). No front-end is needed.

Business Requirements
each entity has an associated image file
create a new entity
modify an existing entity
delete an entity
get entity details (including images)
list all entities

Technical requirements
Spring Boot
Java 11
Swagger

AWS requirements
multi-region
VPC with IGW
there are subnets and security groups as well
endpoints are accessible from the public internet (sec group and NACL is configured properly)
images are stored in S3 and served by CloudFront
by default there is one EC2 in each subnet, but its wrapped with an ASG and can scale to max 3 instances (scaling strategy/params is your choice)
there is an ELB attached to the ASG
entities are stored in Dynamo DB

Create a demo code that simulates autoscaling (upscale and downscale as well).
