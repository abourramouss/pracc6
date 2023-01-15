FROM nginx:alpine

RUN apk add openjdk17

COPY default.conf /etc/nginx/conf.d/default.conf
COPY website /usr/share/nginx/html/
COPY jar /home/
COPY wrapper.sh /home/wrapper.sh

#CMD ["nginx", "-g", "deamon off;"]
CMD /home/wrapper.sh

#RUN java -jar /home/categoryManagement.jar
#RUN java -jar /home/elementManagement.jar
#RUN java -jar /home/gateway.jar

EXPOSE 8080