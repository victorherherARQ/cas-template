CAS Overlay Template
============================

Generic CAS WAR overlay to exercise the latest versions of CAS. This overlay could be freely used as a starting template for local CAS war overlays. The CAS services management overlay is available [here](https://github.com/apereo/cas-services-management-overlay).

# Versions

```xml
<cas.version>5.2.x</cas.version>
```

# Requirements

* JDK 1.8+
* En server.xml del tomcat habilitar:
```
<Connector SSLEnabled="true" clientAuth="false" keystoreFile="{cas-project}/src/main/resources/etc/cas/thekeystore" keystorePass="changeit" maxThreads="200" port="8443" protocol="org.apache.coyote.http11.Http11NioProtocol" scheme="https" secure="true" sslProtocol="TLS"/>
```
* Tener creado en el equipo los directorios:
- /etc/cas/logs
- /etc/cas/saml


# Configuration

Actualmente está configurado para que registre contra BBDD la recomendación por agilidad es que servicios y ticket persistieran en Redis.


