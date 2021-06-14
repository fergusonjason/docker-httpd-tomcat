# docker-nginx-tomcat

This is my Docker project to create a Tomcat Cluster with an NGINX frontend to load-balance it. It was originally based on the work of Paritosh Anand and his project located at https://github.com/Paritosh-Anand/Docker-Httpd-Tomcat (before I switched from HTTPD and squished the tomcat config to one directory).

TODO List:
- ~~One tomcat configuration to rule them all and in the darkness bind them~~
- ~~Switch to alpine images~~ (Foolish me, there ARE no alpine versions of Tomcat)
- ~~Activate Manager on tomcat nodes so I can deploy app via Maven Cargo~~
- ~~Switch over to nginx since the apache and mod_jk guys decided to make this as difficult as humanly possible~~
- Map the log files over to the host from the container
