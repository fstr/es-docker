```
docker run --rm -d \
--name "wbs-prod-elastic" \
-p 9200:9200 \
-v /usr/share/elasticsearch/data:/usr/share/elasticsearch/data \
--memory="4g" \
-e ES_HEAP_SIZE=2g \
elastic-image
```
