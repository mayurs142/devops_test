FROM jboss/wildfly

USER root

ENV jbossDir=/opt/jboss/wildfly/standalone/deployments

ADD companyNews.war ${jbossDir}

RUN mkdir -p /Users/dcameron/persistence/files \
    && touch ${jbossDir}/companyNews.war.dodeploy

EXPOSE 8080