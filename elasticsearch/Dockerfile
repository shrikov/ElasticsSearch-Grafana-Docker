FROM docker.elastic.co/elasticsearch/elasticsearch:8.11.0

# Just set memory limit and run as single node
ENV discovery.type=single-node
ENV ES_JAVA_OPTS="-Xms512m -Xmx512m"

EXPOSE 9200
