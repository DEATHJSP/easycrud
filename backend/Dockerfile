FROM maven:3.8.3-openjdk-17

copy . /op/

workdir /opt

run cp -f application.properties src\main\resources\application.properties

run mvn clean package

workdir /opt/target

expose 8080

ENTRYPOINT [ "java","-jar" ]
CMD [ "student-registration-backend-0.0.1-SNAPSHOT.jar" ]
