# spring-boot-starter-netty
[[English]](https://github.com/Leibnizhu/spring-boot-starter-netty/blob/master/README.md) [[中文]](https://github.com/Leibnizhu/spring-boot-starter-netty/blob/master/README.zh.md)  
## Introduction
This is a Spring Boot embedded servlet container project base on netty API (4.1.12.Final).  

## Maven Dependencies
1. clone this project, 
2. run:  
```
mvn install
```
3. add the dependencies below to your maven project:
```xml
<dependencies>
    <!-- exludes embedded Tomcat -->
    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-web</artifactId>
        <exclusions>
            <exclusion>
                <groupId>org.springframework.boot</groupId>
                <artifactId>spring-boot-starter-tomcat</artifactId>
            </exclusion>
        </exclusions>
    </dependency>
    <!-- include this netty servlet container -->
    <dependency>
        <groupId>io.gitlab.leibnizhu</groupId>
        <artifactId>spring-boot-starter-netty</artifactId>
        <version>1.0-SNAPSHOT</version>
    </dependency>
</dependencies>
```
I'm trying to add this project into maven center repository, please wait.  

## Blogs about how to design/code this project
Only Chineses, updating one after another……  
[基于Netty的Spring Boot内置Servlet容器的实现（一）](http://leibnizhu.gitlab.io/2017/08/24/%E5%9F%BA%E4%BA%8ENetty%E7%9A%84Spring%20Boot%E5%86%85%E7%BD%AEServlet%E5%AE%B9%E5%99%A8%E7%9A%84%E5%AE%9E%E7%8E%B0%EF%BC%88%E4%B8%80%EF%BC%89/)  
[基于Netty的Spring Boot内置Servlet容器的实现（二）](http://leibnizhu.gitlab.io/2017/08/24/%E5%9F%BA%E4%BA%8ENetty%E7%9A%84Spring-Boot%E5%86%85%E7%BD%AEServlet%E5%AE%B9%E5%99%A8%E7%9A%84%E5%AE%9E%E7%8E%B0%EF%BC%88%E4%BA%8C%EF%BC%89/)  
[基于Netty的Spring Boot内置Servlet容器的实现（三）](http://leibnizhu.gitlab.io/2017/08/27/%E5%9F%BA%E4%BA%8ENetty%E7%9A%84Spring-Boot%E5%86%85%E7%BD%AEServlet%E5%AE%B9%E5%99%A8%E7%9A%84%E5%AE%9E%E7%8E%B0%EF%BC%88%E4%B8%89%EF%BC%89/)  

