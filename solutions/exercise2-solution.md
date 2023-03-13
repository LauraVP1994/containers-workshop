# Solution exercise 2

```
docker run --rm -it -v ~/containers/data/:/data quay.io/biocontainers/fastqc:0.11.9--0 /bin/bash 
```
I did: 
```
docker run --rm -it -v $(pwd)/data/:/data quay.io/biocontainers/fastqc:0.11.9--0 /bin/bash
cd data
ls
```



```
docker run --rm -v ~/containers/data/:/data quay.io/biocontainers/fastqc:0.11.9--0 fastqc /data/ecoli_1.fastq.gz
```

Answer: The fastqc within the container only sees its own environment and it is located in /data

or 
```
docker run --rm -v $(pwd)/data/:/data quay.io/biocontainers/fastqc:0.11.9--0 fastqc /data/ecoli_1.fastq.gz
```
