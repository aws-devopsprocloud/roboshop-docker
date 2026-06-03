FROM maven:3.9.14
EXPOSE 8080 
WORKDIR /opt/server 
ENV CART_ENDPOINT="cart:8080"
ENV DB_HOST="mysql""
COPY src/ /opt/server/src
COPY pom.xml /opt/server 
RUN mvn clean package 
RUN mv target/shipping-1.0.jar shipping.jar 
CMD ["java", "-jar", "shipping.jar"]
