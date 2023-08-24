FROM nginx

COPY ./default.conf /etc/nginx/conf.d/default.conf

RUN mkdir -p /usr/share/nginx/html/health \
&& echo '{"status": "OK"}' > /usr/share/nginx/html/health/index.json

CMD ['service', 'nginx', 'start']
