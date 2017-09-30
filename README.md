```
docker run -d \
--name "wbs-prod-elastic" \
--restart unless-stopped \
-p 127.0.0.1:9200:9200 \
-v /usr/share/elasticsearch/data:/usr/share/elasticsearch/data \
-v /usr/share/elasticsearch/logs:/usr/share/elasticsearch/logs \
--memory="4g" \
-e ES_HEAP_SIZE=2g \
elastic-image
```
