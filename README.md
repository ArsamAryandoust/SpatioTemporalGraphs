# Tackling climate change using spatio-temporal graphs for automated deep learning


## Jupyter notebooks inside docker containers

Build Jupyter notebook container:
``` 
docker build -t main_notebook DockerNotebook
```

For CPU computation run:
``` 
docker run -it -v ~/SpatioTemporalGraphs:/SpatioTemporalGraphs -p 3333:1111 main_notebook
```

For GPU computation run:
``` 
docker run -it --gpus all -v ~/SpatioTemporalGraphs:/SpatioTemporalGraphs -p 3333:1111 main_notebook
```
