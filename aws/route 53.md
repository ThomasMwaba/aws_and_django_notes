## Route 53

* Is a DNS (Domain Name System) Service

* DNS is used to help users connect to infrastructure on AWS.

### The most common use case:

>>> Domain name registration 

>>> * .com
>>> * .net
>>> * .org

for example, mydomainname.com

### DNS Records

* Records allows us to choose how we want to route traffic to a domain.

* Each Record has got:

>>> 1. Domain/Subdomain name - for example, mydomain.com

>>> 2. Record Types - for example , A or AAAA

>>> 3. Value - for example , 12.34.56.78

>>> 4. Routing Policy - how Route 53 responds to DNS queries

>>> 5. TTL - amount of time the read cached at DNS resolvers

### Some common DNS Record Types

| Record | Description| Example |
|----------|----------|----------|
| A   | Maps a hostname to IPv4  | 192.0.2.1  |
| AAAA    | Maps a hostname to IPv6  | 2001:0db8:85a3:0:0:8a2e:0370:7334 |
| CNAME    | Maps a hostname to another hostname   | hostname.example.com  |
| ALIAS    | Maps a hostname to an AWS Resource   | CloudFront & S3 Buckets |

-- Add TABLE

### Route 53 - Routing Policies

>> Routing polices help us define how Route 53 responds to DNS queries.

##### Some Common Routing Policies 

| Policy | Description|
|----------|----------|
| Simple  | It is commonly used to route traffic to a single resource |
| Weighted  | It is used to control the percent of requests that go to each specific resource |
| Latency   | Is used to redirect clients to the resource with the least latency(delay) |
| Geolocation   | Is different from Latency. The routing is based on user location( continent, country or state)   |






 ##### Sources

 >>>> * [AWS Documentation](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-dns.html)

 >>>> * [Python Django For AWS Development - Mastery Course - Part 1](https://www.udemy.com/course/python-django-for-aws-development-mastery-course-part-1/?kw=arno&src=sac)

  >>>> * [Ultimate AWS Certified Developer Associate 2024 NEW DVA-C02](https://www.udemy.com/course/aws-certified-developer-associate-dva-c01/?kw=aws+develop&src=sac&couponCode=LEADERSALE24TRFR)


