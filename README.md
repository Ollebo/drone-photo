# drone-photo

Repo with docs how to process images the best way 

## Make Digitail images


```
docker run -ti --rm -v $PWD:/datasets/code opendronemap/odm \
	--project-path /datasets \
	--orthophoto-resolution 1 \
	--skip-3dmodel \
	--skip-report \
	--rerun-all  \
	--feature-quality ultra \
	--orthophoto-compression NONE\
        --smrf-window 3\
	--mesh-octree-depth 11\
	--orthophoto-resolution 1.8\
	--dtm \
	--dem-resolution 7\
	--ignore-gsd\
	--dsm \
	--camera-lens brown\
	--smrf-threshold 3 \
```



## Make orthophoto hig quality

```
docker run -ti --rm -v $PWD:/datasets/code opendronemap/odm --project-path /datasets --orthophoto-resolution 5 --skip-3dmodel --skip-report --rerun-all  --feature-quality ultra --ignore-gsd
```