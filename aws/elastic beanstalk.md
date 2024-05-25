## Elastic Beanstalk

allows the developer to only focus on deploying their application by taking care of all the infrastructure (EC2 instances, Elastic load balancer, Auto scaling Group, Relational Databases etc.) for us



### Configuration

* To Provide integration with Git 
Note: it needs to be installed globally 

>>![Example Image](images/awsebcli.png)


* To take care of the communication between Django application and web server.

>>![Example Image](images/gunicorn.png)



### Deployment Preparation For Elastic Beanstalk

>>![Example Image](images/requirements.png)

Creates a requirements.txt file with all the packages and dependencies



### Deploying An Application To Elastic Beanstalk

1. Create a .ebextensions folder in the directory.


2. Which will have a .config file used to communicate between Elastic Beanstalk and the Django application itself.

```
    option_settings:
    aws:elasticbeanstalk:container:python:
    WSGIPath: application_name.wsgi:application
```

Creates a python container on elasticbeanstalk based on WSGIPATH

3. For the next step make sure you are not in the venv environment.

"ven/Scripts/deactivate"

4. 


| Commands | Description|
|----------|----------|
| eb init   | creates the application  | 
| eb create   | creates the environment  | 
| eb  open  | helps us open the link to the application  |


 ##### Sources

 >>>> * [AWS Documentation](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/Welcome.html)

 >>>> * [Python Django For AWS Development - Mastery Course - Part 1](https://www.udemy.com/course/python-django-for-aws-development-mastery-course-part-1/?kw=arno&src=sac)

  >>>> * [Ultimate AWS Certified Developer Associate 2024 NEW DVA-C02](https://www.udemy.com/course/aws-certified-developer-associate-dva-c01/?kw=aws+develop&src=sac&couponCode=LEADERSALE24TRFR)