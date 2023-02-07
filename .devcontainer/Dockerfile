FROM mcr.microsoft.com/devcontainers/javascript-node

# Install latest pnpm
RUN npm install -g pnpm

# Install deno
RUN curl -fsSL https://deno.land/x/install/install.sh | sh

# Install playwright
RUN mkdir /tmp/pwt && cd /tmp/pwt && npm install @playwright/test && npx playwright install chrome

COPY welcome-message.txt /usr/local/etc/vscode-dev-containers/first-run-notice.txt