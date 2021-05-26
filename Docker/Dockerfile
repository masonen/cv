FROM node:14-alpine

WORKDIR /data

ENV PUPPETEER_SKIP_DOWNLOAD=true \
    NODE_MODULES_PATH="/usr/local/lib/node_modules"

RUN npm install -g resume-cli \
    && sed -i~ "s/localhost/0.0.0.0/g" ${NODE_MODULES_PATH}/resume-cli/build/serve.js

CMD ["resume", "serve", "--theme", "kendall"]