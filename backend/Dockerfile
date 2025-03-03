FROM node:20
WORKDIR /opt/backend
COPY scripts/* .
RUN npm install
ENV DB_HOST="mysql"
CMD ["node", "index.js"]