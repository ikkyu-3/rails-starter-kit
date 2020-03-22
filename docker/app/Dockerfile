FROM ruby:2.7

RUN \
    # Node.js
    curl -sL https://deb.nodesource.com/setup_12.x | bash - && \
    # Yarn
    curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add - && \
    echo "deb https://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list && \
    # apt install
    apt update && apt upgrade && \
    apt install nodejs yarn && \
    # gem
    gem install bundler sqlite3 rails:6.0

WORKDIR /usr/src/my-app