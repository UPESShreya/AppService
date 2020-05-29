FROM java:8
VOLUME /tmp
ADD target/resturant-service-0.0.1-SNAPSHOT.jar usr/app.jar
WORKDIR usr/
RUN bash -c 'touch app.jar'
ENTRYPOINT ["java","-Dspring.data.mongodb.uri=mongodb://localhost:27017/restaurantdb","-jar","app.jar"]