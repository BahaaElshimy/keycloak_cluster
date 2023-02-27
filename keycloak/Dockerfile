FROM quay.io/keycloak/keycloak:19.0.3

USER 0

# Add simple custom JGroups configuration
COPY --chown=keycloak:keycloak ./cache-custom.xml /opt/keycloak/conf/cache-custom.xml

USER keycloak

ENTRYPOINT [ "/opt/keycloak/bin/kc.sh" ]