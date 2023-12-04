FROM spark-base:latest

COPY history-server.sh /


ENV SPARK_EVENTLOG_ENABLED true
ENV SPARK_EVENTLOG_DIR file:///tmp/spark-events

EXPOSE 18081

CMD ["/bin/bash", "/history-server.sh"]