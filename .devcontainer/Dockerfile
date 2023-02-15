FROM mcr.microsoft.com/devcontainers/javascript-node

# Install latest pnpm
RUN npm install -g pnpm

# Install deno
RUN curl -fsSL https://deno.land/x/install/install.sh | sh

# Install playwright
RUN npx playwright install chromium

COPY welcome-message.txt /usr/local/etc/vscode-dev-containers/first-run-notice.txt