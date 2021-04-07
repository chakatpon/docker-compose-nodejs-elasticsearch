FROM docker.elastic.co/kibana/kibana:7.4.0


COPY entrypoint.sh /tmp/entrypoint.sh
RUN chmod -R a+X /tmp/entrypoint.sh

RUN kibana plugin --install elastic/sense

CMD ["/tmp/entrypoint.sh"]
