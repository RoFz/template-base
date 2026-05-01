FROM mcr.microsoft.com/devcontainers/base:ubuntu

RUN apt-get update \
    && apt-get install -y --no-install-recommends gnupg2 pipx python3-pip \
    && rm -rf /var/lib/apt/lists/*

RUN mkdir -p /home/vscode/.claude /home/vscode/.codex /home/vscode/.gnupg /home/vscode/.vscode-server \
    && chown vscode:vscode /home/vscode/.claude /home/vscode/.codex /home/vscode/.gnupg /home/vscode/.vscode-server \
    && chmod 700 /home/vscode/.gnupg \
    && chmod 777 /home/vscode/.vscode-server
