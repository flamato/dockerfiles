#
# Fiji + Java 6 Dockerfile
#

# Pull base JDK-6 image.
FROM dockerfile/java:oracle-java6

# Define maintainer.
MAINTAINER Mark Hiner <hinerm@gmail.com>

# Define working directory.
WORKDIR /fiji

# Install Fiji.
RUN \
      curl -O http://update.imagej.net/bootstrap.js && \
      jrunscript bootstrap.js update-force-pristine

# Add fiji to the PATH
ENV PATH $PATH:/fiji

# Define default command.
CMD ["fiji-linux64"]
