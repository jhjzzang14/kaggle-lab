### 머신러닝 도커 환경 구축

```bash
# docker image 받기
docker build -t deep_learning .

# 이미지 실행
docker run -d -p 8888:8888  -it -v $(pwd):/app deep_learning /bin/bash

# 쥬피터 실행
jupyter notebook --ip 0.0.0.0 --port 8888 --allow-root --no-browser &
```