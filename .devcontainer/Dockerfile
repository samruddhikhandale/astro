FROM mcr.microsoft.com/devcontainers/universal:2

# Install latest pnpm
RUN npm install -g pnpm

# Install deno
ENV DENO_INSTALL=/usr/local
RUN curl -fsSL https://deno.land/x/install/install.sh | sh

# Install playwright
RUN npm install @playwright/test && npx playwright install chrome

COPY welcome-message.txt /usr/local/etc/vscode-dev-containers/first-run-notice.txt