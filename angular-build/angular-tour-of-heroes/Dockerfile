FROM nginx:alpine

# Clean default nginx html files
RUN rm -rf /usr/share/nginx/html/*

# Copy Angular build output
COPY ./browser /usr/share/nginx/html/

# Copy custom nginx config (make sure nginx.conf exists in your project)
COPY ./nginx.conf /etc/nginx/conf.d/default.conf

ARG argValue
ARG argValueWithDefaultValue=the_default_Value_of_the_arg

LABEL labelOne=label_default
LABEL labelTwo=${argValueWithDefaultValue}


RUN echo '=================================='
RUN echo ${argValueWithDefaultValue}
RUN echo $envValue
RUN echo '=================================='

# (Optional) Add extra icon file
#ADD https://www.docker.com/app/uploads/2024/01/icon-dokcer-square.svg /usr/share/nginx/html/

EXPOSE 80

HEALTHCHECK --interval=30s --timeout=10s --start-period=5s --retries=3 \
    CMD curl -f https://localhost/ || exit 1

# Start nginx
CMD ["nginx", "-g", "daemon off;"]
