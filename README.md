# Three Teir AWS Web Application

### Descreption:

Deploying simple  three tier web application on AWS using set of AWS services creating creating the necessary network, security, app, and database components and configurations in order to run this architecture in an available and scalable manner.

### Architecture overview :

In this architecture [3tierArch](https://github.com/sara123-mo/project-1/blob/main/3TierArch.png), a public-facing Application Load Balancer forwards client traffic to our web tier EC2 instances. The web tier is running Nginx webservers that are configured to serve a React.js website and redirects our API calls to the application tier’s internal facing load balancer. The internal facing load balancer then forwards that traffic to the application tier, which is written in Node.js. The application tier manipulates data in an Aurora MySQL multi-AZ database and returns it to our web tier. Load balancing, health checks and autoscaling groups are created at each layer to maintain the availability of this architecture.

### Worshop link :
https://catalog.us-east-1.prod.workshops.aws/workshops/85cd2bb2-7f79-4e96-bdee-8078e469752a/en-US


