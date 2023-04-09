FROM quay.io/keycloak/keycloak-x:15.0.2
WORKDIR /opt/keycloak

ENV KEYCLOAK_ADMIN=abc
ENV KEYCLOAK_ADMIN_PASSWORD=abc
ENV KC_HOSTNAME=localhost:8080

ADD ./realm-config.json ./

EXPOSE 8080

CMD ["start-dev","-Dkeycloak.import=/opt/keycloak/realm-config.json"]

