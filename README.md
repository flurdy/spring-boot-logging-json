# Logging JSON

Outputs console logging as JSON for easier ELK integration.

Useful in clustered environments e.g. Kubernetes, where fluentd or similar reads containers stdout for logs.


Source at https://github.com/flurdy/spring-boot-logging-json

Builds at https://circleci.com/gh/flurdy/spring-boot-logging-json

Jars at https://bintray.com/flurdy/maven/spring-boot-logging-json

In maven:

    <repository>
      <snapshots>
        <enabled>false</enabled>
      </snapshots>
      <id>bintray-flurdy-maven</id>
      <name>bintray</name>
      <url>https://dl.bintray.com/flurdy/maven</url>
    </repository>



    <dependency>
      <groupId>com.flurdy</groupId>
      <artifactId>spring-boot-logging-json</artifactId>
      <version>1.0</version>
    </dependency>

In Gradle:


    repositories {
        maven { 
            url "https://dl.bintray.com/flurdy/maven" 
        }
    }


    dependencies {
        compile 'com.flurdy:spring-boot-logging-json:1.0'
    }

