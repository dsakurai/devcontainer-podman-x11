FROM debian:stable-slim

RUN apt update && \
    apt install -y git curl vim sudo && \
    # Clean up apt cache when done
    rm -rf /var/lib/apt/lists/*

# For VSCode
RUN adduser --disabled-password --gecos "" vscode

# For doing sudo operations (rather dangerous)
# RUN adduser vscode sudo && \
#    echo "vscode ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers.d/nopasswd

USER vscode
