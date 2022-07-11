FROM alpine:3.6

WORKDIR /app/back-end/
COPY ./node_modules.tar.gz ./
COPY ./ ./
EXPOSE 3001
ENTRYPOINT [ "npm" ]
CMD ["start"]
