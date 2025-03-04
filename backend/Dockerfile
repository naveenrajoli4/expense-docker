FROM node:20
WORKDIR /opt/backend
COPY scripts/* .
RUN npm install
# ENV DB_HOST="mysql"
# ENV DB_HOST="localhost" ---> this form host network
ENV DB_HOST="localhost" 
CMD ["node", "index.js"]