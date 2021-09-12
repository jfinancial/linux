## Prerequisites for Production

1. Infrastructure
   - [Install on configure DNS Bind](https://serverspace.io/support/help/configure-bind9-dns-server-on-ubuntu/)
   - [Nginx reverse proxy setup](http://jasonwilder.com/blog/2014/03/25/automated-nginx-reverse-proxy-for-docker/)
   - Set up [Nginx as reverse proxy](http://oskarhane.com/nginx-as-a-reverse-proxy-in-front-of-your-docker-containers/)
   - Or [HaProxy as a static reverse proxy for Docker](http://oskarhane.com/haproxy-as-a-static-reverse-proxy-for-docker-containers/)
   - [Fixed local IP for build box](https://linuxconfig.org/how-to-configure-static-ip-address-on-ubuntu-18-10-cosmic-cuttlefish-linux/)
   - [Install Harbor on NAS](https://www.codetd.com/en/article/11666246)   
   - [Upgrade Synology Diskstation DS418 => DS920+ or DS1520+](https://nascompares.com/2020/08/26/synology-ds1520-vs-ds920-nas-drive-comparison/)
   - [Gitlab on a Diskstation](https://mlohr.com/gitlab-on-a-diskstation/)
   - [Set up local domains](https://www.interserver.net/tips/kb/local-domain-names-ubuntu/)


2. Create CI Pipeline
   - Set up [Gitlab running under Docker](https://github.com/mgcrea/docker-compose-gitlab-ce)
   - [Synology Git](https://www.synology.com/en-uk/dsm/packages/Git)
   - [Synology GitLab](https://www.synology.com/en-uk/dsm/packages/Docker-GitLab) works on [Synology Diskstation DS1520+ NAS](https://www.scan.co.uk/products/5-bay-synology-diskstation-ds1520plus-intel-celeron-j4125-quad-core-8gb-ddr4-2x-m2-slots-25-35-4x-gb)
   - [Set up Git on NAS](https://gist.github.com/walkerjeffd/374750c366605cd5123d)
   - [Setup on OSS Sonar Nexus on NAS](http://www.jamielaing.com/2020/01/so-it-took-me-while-to-find-this-so-i.html)

   - Git availability?


3. Install SSO / [CAS](https://cwiki.apache.org/confluence/pages/viewpage.action?pageId=66427) 
    - [Apache Apereo](https://github.com/apereo/cas) in [Docker](https://hub.docker.com/r/apereo/cas/)
    - Cerificates?


4. Install Docker
   
   - Follow [Instructions](https://github.com/alexisrolland/docker-postgresql-postgraphile)
   1. `$ sudo apt-get update`
   2. `$ sudo apt-get install docker-ce`  
   3. `$ sudo usermod -a -G docker <username>` => Add your user to the docker group to setup its permissions. (Make sure to restart your machine after executing this command.)
   4. `$ sudo apt install docker-compose`
   

5. Deploy to Prod
   - [Deploy to EC2](https://www.youtube.com/watch?v=vmbhFZJUTR0)
   
6. Cloud Services Required
   1. Eureka
   2. Spring Cloud Config Server
   3. Postgres
   4. Posgraphile

    




