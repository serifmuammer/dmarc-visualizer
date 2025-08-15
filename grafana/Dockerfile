#FROM grafana/grafana:8.5.9
FROM grafana/grafana:9.5.21

COPY --chown=grafana:root dashboards/ /var/lib/grafana/dashboards/
RUN chmod 644 /etc/grafana/provisioning

COPY grafana-provisioning/ /etc/grafana/provisioning/
COPY plugins/ /var/lib/grafana/plugins/