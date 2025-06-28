# Use official Apache Tomcat image with Java 17
FROM tomcat:9-jdk17

# Remove default apps from Tomcat (optional but clean)
RUN rm -rf /usr/local/tomcat/webapps/*

# Copy your WAR file into Tomcat webapps as ROOT.war
COPY target/*.war /usr/local/tomcat/webapps/ROOT.war

# Expose port 8080 (used by Tomcat)
EXPOSE 8080
