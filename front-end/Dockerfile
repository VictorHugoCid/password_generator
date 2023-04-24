FROM node

WORKDIR /tmp/react

COPY . .

RUN npm i

RUN npm run build

RUN mkdir -p /var/www/html

# RUN mv build/* /var/www/html tem q ser dist no lugar de build
RUN mv dist/* /var/www/html #tem q ser dist no lugar de build

WORKDIR /

RUN rm -rf /tmp/react