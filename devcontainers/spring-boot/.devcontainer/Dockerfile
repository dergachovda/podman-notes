FROM mcr.microsoft.com/devcontainers/java:25

# ensure JAVA_HOME is explicit for tools like Gradle and VS Code
ENV JAVA_HOME=/usr/lib/jvm/msopenjdk-current
ENV PATH=$JAVA_HOME/bin:$PATH

# Gradle wrapper cache
RUN mkdir -p /root/.gradle

# Optional: Install additional packages
RUN apt-get update && apt-get install -y \
    curl \
    httpie \
    && rm -rf /var/lib/apt/lists/*
