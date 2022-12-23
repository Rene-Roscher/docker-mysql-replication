FROM mysql:5.7
ENV REPLICATION_USER replication
ENV REPLICATION_PASSWORD replication_pass
COPY docker/replication-entrypoint.sh /replication-entrypoint.sh
COPY docker/init-slave.sh /init-slave.sh
RUN chmod +x replication-entrypoint.sh
ENTRYPOINT ["./replication-entrypoint.sh"]
CMD ["mysqld"]
