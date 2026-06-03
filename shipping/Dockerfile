FROM maven:3.9.14
EXPOSE 8080 
WORKDIR /opt/shipping 
ENV CART_ENDPOINT="cart:8080"
ENV DB_HOST="mysql"
COPY src/ /opt/shipping/src/
COPY pom.xml /opt/shipping
RUN mvn clean package 
RUN mv target/shipping-1.0.jar shipping.jar 
CMD ["java", "-jar", "shipping.jar"]


# FROM maven:3.9.14
# EXPOSE 8080
# WORKDIR /app
# COPY pom.xml .
# COPY src ./src
# RUN mvn clean package 
# RUN mv target/shipping-1.0.jar shipping.jar 
# ENV CART_ENDPOINT="cart:8080" \
#     DB_HOST="mysql"
# CMD ["java", "-jar", "shipping.jar"]