# Docker image for HSSM

To build image

```
docker build -t zenkavi/hssm:0.0.2 -f Dockerfile .
```

To run notebooks in container

```
docker run -it --rm \
-v $(pwd):/home/jovyan/work \
-p 8888:8888 zenkavi/hssm:0.0.2 jupyter notebook
```

## Acknowledgement

Thanks [Hu Chuan-Peng](https://github.com/hcp4715) for the [dockerHDDM image](https://github.com/hcp4715/dockerHDDM). This HSSM image heavily relied on his Dockerfile.