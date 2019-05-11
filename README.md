#A sample project for testing/demonstrating keycloak features

1. **Avoid requiring HTTPS**  
(within docker container)  
`cd /opt/jboss/keycloak/bin/ && ./kcadm.sh config credentials --server http://localhost:8080/auth --realm master --user $KEYCLOAK_USER --password $KEYCLOAK_PASSWORD && ./kcadm.sh update realms/master -s sslRequired=NONE`
