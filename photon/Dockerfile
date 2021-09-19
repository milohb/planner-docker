FROM adoptopenjdk/openjdk11:alpine-jre

RUN mkdir -p /usr/local/photon/datadir
ENV JAVA_OPTIONS=-Xmx8G

COPY photon-0.3.5.jar /usr/local/photon

EXPOSE 2322

ENTRYPOINT ["/bin/sh", "-c"]
CMD ["java $JAVA_OPTIONS -jar /usr/local/photon/photon-0.3.5.jar -data-dir /usr/local/photon/datadir"]
