FROM adoptopenjdk/openjdk11:alpine-jre
LABEL authors="Stepan Kuzmin <to.stepan.kuzmin@gmail.com>, Sandeep Pandey <spandey.ike@gmail.com, Michael Lorenzen <ml@m-lorenzen.de"

ENV OTP_VERSION=2.0.0
ENV JAVA_OPTIONS=-Xmx4G

ADD otp-2.jar /usr/local/share/java/

RUN mkdir -p /var/opt/graphs
RUN ln -s otp-2.jar /usr/local/share/java/otp.jar

COPY otp /usr/local/bin

EXPOSE 8080

ENTRYPOINT ["otp"]
CMD ["--help"]
