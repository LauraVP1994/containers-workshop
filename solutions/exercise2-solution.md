# Solution exercise 2

```
docker run --rm -it -v ~/containers/data/:/data quay.io/biocontainers/fastqc:0.11.9--0 /bin/bash 
```

```
docker run --rm -v ~/containers/data/:/data quay.io/biocontainers/fastqc:0.11.9--0 fastqc /data/WT_lib1_R1.fq.gz
```
