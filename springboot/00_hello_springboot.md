# 00\_HELLO\_SPRINGBOOT

### 1. 프로젝트 생성

#### 1-1. IntelliJ에서 SpringBoot 프로젝트 생성하

![](../.gitbook/assets/image%20%283%29.png)

![](../.gitbook/assets/image%20%284%29.png)

#### 1-2. Gradle 프로젝트를 Spring 프로젝트로 변경

```text
buildscript {
    ext {
        springBootVersion = '2.1.7.RELEASE'
    }
    repositories {
        mavenCentral()
        jcenter()
    }
    dependencies {
        classpath("org.springframework.boot:spring-boot-gradle-plugin:${springBootVersion}")
    }
}

apply plugin: 'java'
apply plugin: 'eclipse'
apply plugin: 'org.springframework.boot'
apply plugin: 'io.spring.dependency-management'

group 'hello-springboot'
version '1.0-SNAPSHOT'
sourceCompatibility = 1.8

repositories {
    mavenCentral()
}

dependencies {
    compile('org.springframework.boot:spring-boot-starter-web')
    testCompile('org.springframework.boot:spring-boot-starter-test')
}
```



