## Hands-On Time

---

# Instrumenting Services


## Histograms

---

```bash
open "https://goo.gl/jc6aUx"

curl -L -o go-demo.yml https://goo.gl/eoP7zE

cat go-demo.yml

docker stack deploy -c go-demo.yml go-demo

open "http://$(docker-machine ip swarm-1)/monitor/alerts"

docker stack ps -f desired-state=running go-demo

open "http://$(docker-machine ip swarm-1)/monitor/targets"

open "http://$(docker-machine ip swarm-1)/monitor/graph"

# sum(rate(http_server_resp_time_bucket{job="go-demo_main",le="0.1"}[5m])) / sum(rate(http_server_resp_time_count{job="go-demo_main"}[5m]))
```
