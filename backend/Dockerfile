FROM node:20
WORKDIR /opt/backend
COPY scripts/* .
RUN npm install
ENV DB_HOST="mysql"
# The below command is used for host network
# ENV DB_HOST="localhost" 
CMD ["node", "index.js"]