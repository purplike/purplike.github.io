---
layout: post
title:  "Spring Boot - Web - 2 - index"
date:   2020-09-16 15:14:00
categories: Spring Boot
---

# pom.xml
처음에 web
thymeleaf 추가

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
	<artifactId>cont</artifactId>
	<version>0.0.1-SNAPSHOT</version>
	<name>cont</name>
	<description>Demo project for Spring Boot</description>

	<properties>
		<java.version>1.8</java.version>
	</properties>

	<dependencies>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-thymeleaf</artifactId>
		</dependency>
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

# IndexController.java
```Java
package com.example.demo;

import org.springframework.stereotype.Controller;
import org.springframework.web.bind.annotation.GetMapping;

@Controller
public class IndexController {

	@GetMapping("/")
	public String index() {
		return "index";
	}
}
```

# src/main/resources
## template/index.html
spring boot 동작후
```Shell
  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::        (v2.3.3.RELEASE)

2020-09-16 15:07:08.826  INFO 58968 --- [           main] com.example.demo.ContApplication         : Starting ContApplication on DESKTOP-G1M4NJ8 with PID 58968 (D:\sts\sts-4.7.0.RELEASE\workspace\test\cont\target\classes started by Maria in D:\sts\sts-4.7.0.RELEASE\workspace\test\cont)
2020-09-16 15:07:08.828  INFO 58968 --- [           main] com.example.demo.ContApplication         : No active profile set, falling back to default profiles: default
2020-09-16 15:07:09.642  INFO 58968 --- [           main] o.s.b.w.embedded.tomcat.TomcatWebServer  : Tomcat initialized with port(s): 8080 (http)
2020-09-16 15:07:09.651  INFO 58968 --- [           main] o.apache.catalina.core.StandardService   : Starting service [Tomcat]
2020-09-16 15:07:09.651  INFO 58968 --- [           main] org.apache.catalina.core.StandardEngine  : Starting Servlet engine: [Apache Tomcat/9.0.37]
2020-09-16 15:07:09.759  INFO 58968 --- [           main] o.a.c.c.C.[Tomcat].[localhost].[/]       : Initializing Spring embedded WebApplicationContext
2020-09-16 15:07:09.759  INFO 58968 --- [           main] w.s.c.ServletWebServerApplicationContext : Root WebApplicationContext: initialization completed in 876 ms
2020-09-16 15:07:09.932  INFO 58968 --- [           main] o.s.s.concurrent.ThreadPoolTaskExecutor  : Initializing ExecutorService 'applicationTaskExecutor'
2020-09-16 15:07:09.996  INFO 58968 --- [           main] o.s.b.a.w.s.WelcomePageHandlerMapping    : Adding welcome page template: index
2020-09-16 15:07:10.138  INFO 58968 --- [           main] o.s.b.w.embedded.tomcat.TomcatWebServer  : Tomcat started on port(s): 8080 (http) with context path ''
2020-09-16 15:07:10.149  INFO 58968 --- [           main] com.example.demo.ContApplication         : Started ContApplication in 1.623 seconds (JVM running for 3.354)

```

# http://localhost:8080/ 접속후

```Shell
2020-09-16 15:07:17.099  INFO 58968 --- [nio-8080-exec-1] o.a.c.c.C.[Tomcat].[localhost].[/]       : Initializing Spring DispatcherServlet 'dispatcherServlet'
2020-09-16 15:07:17.100  INFO 58968 --- [nio-8080-exec-1] o.s.web.servlet.DispatcherServlet        : Initializing Servlet 'dispatcherServlet'
2020-09-16 15:07:17.105  INFO 58968 --- [nio-8080-exec-1] o.s.web.servlet.DispatcherServlet        : Completed initialization in 5 ms

```

