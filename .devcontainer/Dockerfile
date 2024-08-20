FROM ghcr.io/rails/devcontainer/images/ruby:3.3.0

# https://nodejs.org/en/download/package-manager
#RUN curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.0/install.sh | bash \
  #&& export NVM_DIR="$HOME/.nvm" \
  #&& [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" \
  #&& [ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion" \
  #&& nvm install 20 \
  #&& node -v \
  #&& npm -v \
  #&& npm install --global yarn \
  #&& yarn --version

# https://nodejs.org/dist/v20.16.0/node-v20.16.0-linux-x64.tar.xz
ENV PATH="$PATH:/node/node-v20.16.0-linux-x64/bin"
RUN curl -o node-v20.16.0-linux-x64.tar.xz https://nodejs.org/dist/v20.16.0/node-v20.16.0-linux-x64.tar.xz \
 && mkdir /node \
 && tar -xJvf node-v20.16.0-linux-x64.tar.xz -C /node \
 && rm node-v20.16.0-linux-x64.tar.xz \
 && node -v \
 && npm -v \
 && npm install --global yarn \
 && yarn --version
