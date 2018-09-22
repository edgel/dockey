FROM yeahzhu/dockey:tomee

ENV CATALINA_BASE=/usr/local/microc

RUN set -eux; \
  mkdir -p $CATALINA_BASE; \
  \
  mkdir -p $CATALINA_BASE/conf; \
  mkdir -p $CATALINA_BASE/conf/Catalina; \
  chown -R nobody:nogroup $CATALINA_BASE/conf/Catalina; \
  mkdir -p $CATALINA_BASE/conf/conf.d; \
  chown -R nobody:nogroup $CATALINA_BASE/conf/conf.d; \
  mkdir -p $CATALINA_BASE/.well-known; \
  \
  mkdir -p $CATALINA_BASE/logs; \
  chown -R nobody:nogroup $CATALINA_BASE/logs; \
  mkdir -p $CATALINA_BASE/temp; \
  chown -R nobody:nogroup $CATALINA_BASE/temp; \
  mkdir -p $CATALINA_BASE/work; \
  chown -R nobody:nogroup $CATALINA_BASE/work; \
  \
  chown -R nobody:nogroup $CATALINA_BASE/.well-known;

USER nobody
