### Get set up
1. Pull elasticsearch from dockerhub.com
```bash
    docker pull elasticsearch:7.9.2
```
2. Run elasticsearch
```bash
    docker run -d --name elasticsearch -p 9200:9200 -p 9300:9300 -e "discovery.type=single-node" elasticsearch:7.9.2
```
3. Check elasticsearch is running by
```bash
    curl http://www.localhost:9200
```