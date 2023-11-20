# Dockerfile
FROM hashicorp/terraform:0.14.10

LABEL maintainer="Your Name <your.email@example.com>"

# Install additional tools
RUN apk --no-cache add \
    bash \
    curl \
    jq \
    git \
    openssh-client \
    py-pip \
    python3 \
    && pip install --upgrade awscli

# Set the working directory
WORKDIR /app

# Display Terraform version on startup
CMD ["terraform", "version"]
