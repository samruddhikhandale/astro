FROM mcr.microsoft.com/devcontainers/universal:2

# Install latest pnpm
RUN curl -fsSL https://get.pnpm.io/install.sh | SHELL=`which bash` bash -

COPY welcome-message.txt /usr/local/etc/vscode-dev-containers/first-run-notice.txt