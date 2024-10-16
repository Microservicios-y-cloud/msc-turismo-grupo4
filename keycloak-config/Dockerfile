FROM quay.io/keycloak/keycloak:latest as builder

# Enable health and metrics support
ENV KC_HEALTH_ENABLED=true
ENV KC_METRICS_ENABLED=true

WORKDIR /opt/keycloak

ADD --chown=keycloak:keycloak --chmod=644 ./providers/ /opt/keycloak/providers/
ADD --chown=keycloak:keycloak --chmod=644 ./themes/ /opt/keycloak/themes/

RUN /opt/keycloak/bin/kc.sh build 

FROM quay.io/keycloak/keycloak:latest
COPY --from=builder /opt/keycloak/ /opt/keycloak/

ENTRYPOINT ["/opt/keycloak/bin/kc.sh"]