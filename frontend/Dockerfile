FROM nginx
RUN rm -rf /usr/share/nginx/html/*
# RUN rm -rf /etc/nginx/nginx.conf
COPY expense.conf /etc/nginx/nginx.conf
COPY code /usr/share/nginx/html/
CMD ["nginx", "-g", "daemon off;"]