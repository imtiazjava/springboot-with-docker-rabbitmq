# RabbitMQ

![image](https://user-images.githubusercontent.com/26134506/180869852-41d0a428-e301-4dc7-85c0-126eb42beba4.png)

# WHAT IS RABBITMQ?
---------------------------------------------------------------------------
RabbitMQ is an open source message broker written in Java. It's fully compliant with JMS 1.1 standards. It is developed and maintained by Apache Software Foundation and is licensed under Apache license. It provides high availability, scalability, reliability, performance and security for enterprise level messaging applications.

JMS is a specification that allows development of message based system. RabbitMQ acts as a broker of messages which sits in between applications and allows them to communicate in asynchronous and reliable way.

# Installation of RabbiMQ  
    https://www.youtube.com/watch?v=V9DWKbalbWQ
  ---------------------------------------------------------------------------------------------------
  Step1 : https://www.rabbitmq.com/download.html
  
  Step2 : https://www.erlang.org/downloads
  
   ## Install both  the things and once you install the rabbitmq use the following command :
    From the windows search type RabbitMQ it will open the command prompt and type the command as below:
             >rabbitmq-plugins enable rabbitmq_management
             
   ## Now open the  browser type  the URL : http://localhost:15672
                                      USERNAME: Guest
                                      PASSWORD: Guest
                                      
                                     
--------------------------------------------------------------------------------------------------

# Springboot-with-docker-rabbitmq

## Let's Learn how  to implement the SpringBoot with  RabbitMQ
------------------------------------------------------------------
 
 ## Step1: First Install the RabbitMQ with Docker by  using the following command:
         - H:\docker practise>docker run -d --hostname my-rabbit --name some-rabbit -p 15672:15672 -p 5672:5672 rabbitmq:3-management
         - Open  the browser and type the URL : http://localhost:15672
                                UserName: guest
                                Password: guest

# Step2:
## In order to Create the SpringBootWithRabbitMQ application the following programs we need:
     - We have to Create the Queue
     - We have to Create the Exchange
     - And We have to Bind Both Queue and Exchange
     - Finally Pass the Message to the Queue.
     
- First Create ProducerProject
- Then Create the Consumer Project
 
 # spring-rabbitmq-producer project
 - Dependencies:
    ```
   <dependencies>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-amqp</artifactId>
		</dependency>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-web</artifactId>
		</dependency>

		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-devtools</artifactId>
			<scope>runtime</scope>
			<optional>true</optional>
		</dependency>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-test</artifactId>
			<scope>test</scope>
		</dependency>
		<dependency>
			<groupId>org.springframework.amqp</groupId>
			<artifactId>spring-rabbit-test</artifactId>
			<scope>test</scope>
		</dependency>
	</dependencies>
   ```
  --------------------------------------------------------------------------------------------------------------------
 
 
 
  
