SET JAVA_HOME=C:\Program Files\Java\jdk-11.0.1

mvn clean package -Divy.engine.list.url=https://developer.axonivy.com/download/nightly
mvn io.fabric8:docker-maven-plugin:build