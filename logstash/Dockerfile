FROM docker.elastic.co/logstash/logstash:6.5.4

#install the plugin for aggregating log entries
RUN logstash-plugin install logstash-filter-aggregate
RUN rm -r /usr/share/logstash/pipeline
ADD pipeline /usr/share/logstash/pipeline
ADD config/logstash.yml /usr/share/logstash/config/logstash.yml
