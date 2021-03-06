[![Maven Central](https://maven-badges.herokuapp.com/maven-central/com.omnisci/omnisci-jdbc/badge.svg)](https://maven-badges.herokuapp.com/maven-central/com.omnisci/omnisci-jdbc)

## Specifying Maven Dependency

```xml
<dependency>
  <groupId>com.omnisci</groupId>
  <artifactId>omnisci-jdbc</artifactId>
  <version>4.8.0</version>
</dependency>
```

### Before 4.8.0

```xml
<dependency>
  <groupId>com.omnisci</groupId>
  <artifactId>jdbc</artifactId>
  <version>4.7.0</version>
</dependency>
```

## Basic testing
From the top level directory run:
```shell
set +H
mvn test -DskipTests=false -Dtest=!com.omnisci.jdbc.OmniSciConnectionTest#tst1a_binary_encrypted+tst2_http_unencrypted+tst3_https_encrypted+tst4_https_encrypted_with_server_validation
```
*Note: the unit tests assume that local omniscidb is running and default user and database exist*
