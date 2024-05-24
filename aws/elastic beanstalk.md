## Elastic Beanstalk

allows the developer to only focus on deploying their application by taking care of all the infrastructure (EC2 instances, Elastic load balancer, Auto scaling Group, Relational Databases etc.) for us



### Configuration

* To Provide integration with Git 

![Example Image](images/awsebcli.png)

Note: it needs to be installed globally 


![Example Image](images/gunicorn.png)

* Takes care of the communication between Django application and web server.

### Deployment Preparation For Elastic Beanstalk

![Example Image](images/requirements.png)

Creates a requirements.txt file with all the packages and dependencies



### Deploying An Application To Elastic Beanstalk

>>> 1. Domain/Subdomain name - for example, mydomain.com

>>> 2. Record Types - for example , A or AAAA

>>> 3. Value - for example , 12.34.56.78

>>> 4. Routing Policy - how Route 53 responds to DNS queries


| Record | Description| Example |
|----------|----------|----------|
| A   | Maps a hostname to IPv4  | 192.0.2.1  |
| AAAA    | Maps a hostname to IPv6  | 2001:0db8:85a3:0:0:8a2e:0370:7334 |
| CNAME    | Maps a hostname to another hostname   | hostname.example.com  |
| ALIAS    | Maps a hostname to an AWS Resource   | CloudFront & S3 Buckets |


 ##### Sources

 >>>> * [AWS Documentation](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/Welcome.html)

 >>>> * [Python Django For AWS Development - Mastery Course - Part 1](https://www.udemy.com/course/python-django-for-aws-development-mastery-course-part-1/?kw=arno&src=sac)

  >>>> * [Ultimate AWS Certified Developer Associate 2024 NEW DVA-C02](https://www.udemy.com/course/aws-certified-developer-associate-dva-c01/?kw=aws+develop&src=sac&couponCode=LEADERSALE24TRFR)