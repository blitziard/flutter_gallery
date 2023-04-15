FROM ubuntu:latest

# Install dependencies
RUN apt-get update && \
    apt-get install -y curl git unzip xz-utils zip libglu1-mesa

# Install Flutter
RUN git clone https://github.com/flutter/flutter.git /opt/flutter && \
    /opt/flutter/bin/flutter --version

# Enable Flutter web support
RUN /opt/flutter/bin/flutter config --enable-web
