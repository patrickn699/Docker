FROM python:3.7-alpine

ADD . /root/
WORKDIR /app
RUN addgroup -S appgroup && adduser -S appuser -G appgroup
RUN chown -R appuser:appgroup /app
USER appuser
CMD ["cat", "/root/main.py"]