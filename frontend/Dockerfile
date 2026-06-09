FROM nginx:1.24.0 
RUN rm -rf /usr/share/nginx/html/index.html 
COPY static /usr/share/nginx/html/
RUN rm -f /etc/nginx/nginx.conf
RUN rm -f /etc/nginx/conf.d/default.conf
COPY nginx.conf /etc/nginx/nginx.conf



docker push devopsprocloudaws/cart:v1
docker push devopsprocloudaws/catalogue:v1
docker push devopsprocloudaws/frontend:v1
docker push devopsprocloudaws/payment:v1
docker push devopsprocloudaws/shipping:v1
docker push devopsprocloudaws/user:v1
docker push devopsprocloudaws/mongodb:v1
docker push devopsprocloudaws/mysql:v1