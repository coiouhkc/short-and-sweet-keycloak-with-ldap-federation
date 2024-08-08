https://github.com/bitnami/containers/issues/982

https://keycloak.discourse.group/t/how-should-i-sync-groups-from-ad-ldap-to-keycloak/2889


curl -s -d "client_id=mockbin-app" -d "username=mockbin-app-user" -d "password=secret" -d 'grant_type=password' http://keycloak:8080/realms/demo/protocol/openid-connect/token | jq '.access_token'

curl -s -d "client_id=mockbin-app" -d "username=user01" -d "password=secret" -d 'grant_type=password' http://keycloak:8080/realms/demo/protocol/openid-connect/token