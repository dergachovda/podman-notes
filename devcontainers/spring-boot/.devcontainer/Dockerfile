FROM mcr.microsoft.com/devcontainers/java:25

# Gradle wrapper cache
RUN mkdir -p /root/.gradle

# Optional: Install additional packages
RUN apt-get update && apt-get install -y \
    curl \
    httpie \
    && rm -rf /var/lib/apt/lists/*
