FROM openjdk

WORKDIR /app/petclinic
COPY ./* .

ARG APP_DB_DEFAULT=postgres
ENV APP_DB=${APP_DB_DEFAULT}

ARG PORT_DEFAULT=8080
ENV PORT=$PORT_DEFAULT
EXPOSE $PORT_DEFAULT

ENTRYPOINT [ "java", "-Dspring.profiles.active=${APP_DB}", "-jar", "/app/petclinic/petclinic.jar" ]