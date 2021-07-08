# Docker


## Quick Start
[Installation](https://docs.docker.com/engine/install/)


## Docker vs Vm

![https://www.weave.works/blog/a-practical-guide-to-choosing-between-docker-containers-and-vms](./containers-vs-virtual-machines.jpeg)

比較           | VM       | Container
--------------|:---------:|--
啟動速度       | > 3 min.  | 20 sec. < 1 min.
擴充性         | 獨立檔案   | 累進式繼承
擴充性         | 獨立檔案   | 累進式繼承



## Image
 - 映像檔(安裝檔案)
  1. From Reopsitory
  2. Build from DOCKERFILE


## Container
 - 容器：由映像檔產生的執行副本

## Docker Engine
 - 運行容器的環境

## Docker Compose
 - 佈建整套環境的菜單

## Volume
 - 儲存空間

## Network
 - 網路接口



# 實際運行



# 常用指令
[cheatsheet](https://dockerlabs.collabnix.com/docker/cheatsheet/)

  - 查看映像檔
    ```docker images```
  - 查看運行中的容器
    ```docker ps -a```

# 啟動
```sh
docker run -it ubuntu

docker run --rm -it ubuntu

docker run -d ubuntu

docker run --rm -ti \
  -v $(pwd):/src \
  -p 8089:80 \
  dockercloud/hello-world
```
