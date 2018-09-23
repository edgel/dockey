FROM yeahzhu/dockey:tomee

ENV CATALINA_BASE=/usr/local/microc

RUN set -eux; \
  mkdir -p $CATALINA_BASE/conf; \
  chown -R root:root $CATALINA_BASE/conf; \
  \
  mkdir -p $CATALINA_BASE/conf/Catalina; \
  chown -R nobody:nogroup $CATALINA_BASE/conf/Catalina; \
  \
  mkdir -p $CATALINA_BASE/conf/conf.d; \
  chown -R nobody:nogroup $CATALINA_BASE/conf/conf.d; \
  \
  mkdir -p $CATALINA_BASE/temp; \
  chown -R nobody:nogroup $CATALINA_BASE/temp; \
  \
  mkdir -p $CATALINA_BASE/work; \
  chown -R nobody:nogroup $CATALINA_BASE/work; \
  \
  mkdir -p $CATALINA_BASE/logs; \
  chown -R nobody:nogroup $CATALINA_BASE/logs; \
  \
  mkdir -p $CATALINA_BASE/certs; \
  chown -R root:root $CATALINA_BASE/certs; \
  \
  mkdir -p $CATALINA_BASE/webapps; \
  chown -R root:root $CATALINA_BASE/webapps; \
  \
  export source="securerandom\.source\=file\:\/dev\/random"; \
  export target="securerandom\.source\=file\:\/dev\/\.\/urandom"; \
  sed -i "s/$source/$target/g" $JAVA_HOME/lib/security/java.security;

USER nobody
