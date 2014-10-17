General Information
-------------------

Base docker image to run a VIPCON AR Restful API in a Tomcat 8 application server

Usage
-----

To create the image `vipcon/arapi`, execute the following command on the vipcon-arapi folder:

    docker build -t vipcon/arapi .

To run the image and bind to port:

    docker run -d -p 8080:8080 vipcon/arapi
    
To connect to the AR Restful API via the Host:

    http://<docker-host>:8080/arapi
    
!!!Make sure to switch to https if you make the container accessible to others!

About VIPCON AR Restful API
---------------------------

Companies that implemented one or more BMC Remedy ITSM processes store a significant amount of important data about their processes and infrastructure within the BMC Remedy ITSM Suite. It is often desired to use this data in other processes or tools. Sharing this data if often expensive and complicated. Special skills are required to implement interfaces with the BMC Java API. Only a very limited amount of applications are able to integrate with Java natively.

*VIPCON AR Restful API* provides a generic interface to data stored within BMC Remedy ITSM based on todays state of the art integration standard JSON. Nearly all Web Applications and Programming languages can leverage the API natively. It makes integrations faster, easier and cheaper:

* No configuration needed
* Zero code integration possible with many modern Cloud Applications
* Can be deployed in any Web Application Server – even together with MidTier
* Implements Create, Read, Update and Delete operations. Also to attachments
* Reduces implementation costs and time significantly
* Creates value by sharing data across applications and processes
* Can be natively used by Phython, PHP, Java, Shell Scripts, C#, C++ and many more

*VIPCON AR Restful API* supports a variety of use cases like:

* SmartIT & MyIT customization & extension
* Mobil Application integration
* Monitoring CMDB integration 
* Web Application integration
* Cloud Application integration
* *And many more …*


Further information and documentation can be found here

https://communities.bmc.com/docs/DOC-29073

The image is based on the great https://github.com/tutumcloud/tutum-docker-tomcat
