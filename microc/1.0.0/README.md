# Micorc File Structure

/opt/local/tomee (root)/

  bin (root)/

  lib (root)/

  conf (root)/

  temp (root)/

  work (root)/

  logs (root)/

  webapps (root)/

/opt/local/microc (root)/

  conf (root)/

    Catalina (nobody)/

    conf.d (nobody)/

  temp (nobody)/

  work (nobody)/

  logs (nobody)/ <- volume domain-logs/

  certs (root)/ <- volume domain-certs/

  webapps (root)/ <- volume domain-root/webapps/

volume domain-logs/

volume domain-certs/

  webroot/

    .well-known/

volume domain-root/

  webapps/

    domain/

      ROOT/

  start.sh

  stop.sh

  restart.sh

  certs.sh

  recerts.sh

  server.xml

  context.xml

  openejb.xml

  tomee.xml

  tomcat-users.xml

  logging.properties


