# ccaas-langsa-parent
It will be supposed to use in create new project for langsa.

## Publish
```shell
export MAVEN_GPG_PASSPHRASE="timbel****" && \

./mvnw clean package \
  gpg:sign install:install \
  org.sonatype.central:central-publishing-maven-plugin:publish \
  -Dgpg.keyname=95B9EA88 \
  -Dgpg.gpgArguments="--batch,--pinentry-mode,loopback"
```
