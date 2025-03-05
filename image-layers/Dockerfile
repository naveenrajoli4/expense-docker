# FROM node:20
FROM node:20.18-alpine3.21
# addgroup -S appgroup && adduser -S appuser -G appgroup for alpine OS
RUN addgroup -S naveen && adduser -S naveen -G naveen && \
    mkdir /opt/backend && \
    chown -R naveen:naveen /opt/backend
WORKDIR /opt/backend
COPY scripts/* ./
RUN npm install
ENV DB_HOST="mysql"
# The below command is used for host network
# ENV DB_HOST="localhost" 
USER naveen
CMD ["node", "index.js"]