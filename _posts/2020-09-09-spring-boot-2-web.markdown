---
layout: post
title:  "Spring Boot - 2 Web"
date:   2020-09-09 17:46:00
categories: Spring Boot
---

### pom.xml
```XML
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 https://maven.apache.org/xsd/maven-4.0.0.xsd">
	<modelVersion>4.0.0</modelVersion>
	<parent>
		<groupId>org.springframework.boot</groupId>
		<artifactId>spring-boot-starter-parent</artifactId>
		<version>2.3.3.RELEASE</version>
		<relativePath/> <!-- lookup parent from repository -->
	</parent>
	<groupId>com.example</groupId>
	<artifactId>web-1</artifactId>
	<version>0.0.1-SNAPSHOT</version>
	<name>web-1</name>
	<description>Demo project for Spring Boot</description>

	<properties>
		<java.version>1.8</java.version>
	</properties>

	<dependencies>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-web</artifactId>
		</dependency>

		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-test</artifactId>
			<scope>test</scope>
			<exclusions>
				<exclusion>
					<groupId>org.junit.vintage</groupId>
					<artifactId>junit-vintage-engine</artifactId>
				</exclusion>
			</exclusions>
		</dependency>
	</dependencies>

	<build>
		<plugins>
			<plugin>
				<groupId>org.springframework.boot</groupId>
				<artifactId>spring-boot-maven-plugin</artifactId>
			</plugin>
		</plugins>
	</build>

</project>

```

### STS4 Console
```Shell
  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::        (v2.3.3.RELEASE)

2020-09-09 17:28:19.486  INFO 55748 --- [           main] com.example.demo.WebApplication          : Starting WebApplication on DESKTOP-G1M4NJ8 with PID 55748 (D:\sts\sts-4.7.0.RELEASE\workspace\spring-boot\web\target\classes started by Maria in D:\sts\sts-4.7.0.RELEASE\workspace\spring-boot\web)
2020-09-09 17:28:19.491  INFO 55748 --- [           main] com.example.demo.WebApplication          : No active profile set, falling back to default profiles: default
2020-09-09 17:28:20.893  INFO 55748 --- [           main] o.s.b.w.embedded.tomcat.TomcatWebServer  : Tomcat initialized with port(s): 8080 (http)
2020-09-09 17:28:20.907  INFO 55748 --- [           main] o.apache.catalina.core.StandardService   : Starting service [Tomcat]
2020-09-09 17:28:20.908  INFO 55748 --- [           main] org.apache.catalina.core.StandardEngine  : Starting Servlet engine: [Apache Tomcat/9.0.37]
2020-09-09 17:28:21.033  INFO 55748 --- [           main] o.a.c.c.C.[Tomcat].[localhost].[/]       : Initializing Spring embedded WebApplicationContext
2020-09-09 17:28:21.034  INFO 55748 --- [           main] w.s.c.ServletWebServerApplicationContext : Root WebApplicationContext: initialization completed in 1467 ms
2020-09-09 17:28:21.325  INFO 55748 --- [           main] o.s.s.concurrent.ThreadPoolTaskExecutor  : Initializing ExecutorService 'applicationTaskExecutor'
2020-09-09 17:28:21.588  INFO 55748 --- [           main] o.s.b.w.embedded.tomcat.TomcatWebServer  : Tomcat started on port(s): 8080 (http) with context path ''
2020-09-09 17:28:21.605  INFO 55748 --- [           main] com.example.demo.WebApplication          : Started WebApplication in 2.792 seconds (JVM running for 5.702)
2020-09-09 17:28:39.535  INFO 55748 --- [nio-8080-exec-1] o.a.c.c.C.[Tomcat].[localhost].[/]       : Initializing Spring DispatcherServlet 'dispatcherServlet'
2020-09-09 17:28:39.536  INFO 55748 --- [nio-8080-exec-1] o.s.web.servlet.DispatcherServlet        : Initializing Servlet 'dispatcherServlet'
2020-09-09 17:28:39.545  INFO 55748 --- [nio-8080-exec-1] o.s.web.servlet.DispatcherServlet        : Completed initialization in 9 ms
```

### Web
http://localhost:8080/
Whitelabel Error Page
This application has no explicit mapping for /error, so you are seeing this as a fallback.

Wed Sep 09 17:28:39 KST 2020
There was an unexpected error (type=Not Found, status=404).
