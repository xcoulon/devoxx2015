FROM wilfdfly-postgres:9.0.2.Final
MAINTAINER xcoulon@redhat.com

# expose debug port
EXPOSE 8787
EXPOSE 9990

# define the deployments directory as a volume that can be mounted
VOLUME /opt/jboss/wildfly/standalone/deployments

# start WildFly in standalone/debug mode and allow management from host 
CMD ["/opt/jboss/wildfly/bin/standalone.sh", "-c", "standalone.xml", "-b", "0.0.0.0", "-bmanagement", "0.0.0.0" , "--debug"]


