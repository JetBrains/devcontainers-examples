FROM nginx

RUN apt-get update && apt-get install -y procps

EXPOSE 80

STOPSIGNAL SIGQUIT

CMD ["nginx", "-g", "daemon off;"]
