FROM spark-base:latest

COPY start-worker.sh /

ENV SPARK_WORKER_WEBUI_PORT 8081
ENV SPARK_WORKER_LOG /spark/logs
ENV SPARK_MASTER "spark://spark-master:7077"
ENV SPARK_EVENTLOG_ENABLED true
ENV SPARK_EVENTLOG_DIR file:///tmp/spark-events

EXPOSE 8081

CMD ["/bin/bash", "/start-worker.sh"]
