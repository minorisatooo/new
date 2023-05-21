FROM nginx:1.23.0
LABEL org.opencontainers.image.authors="test"

COPY nginx.conf /etc/nginx/nginx.conf

COPY sites-enabled/local-mini-blog.conf /etc/nginx/sites-enabled/local-mini-blog.conf
COPY sites-enabled/default.conf /etc/nginx/conf.d/default.conf

# nginxをdaemon化(background実行)する事を防ぐ nginx:1.23.0で実行されるので不要
# CMD ["nginx", "-g", "daemon off;"]