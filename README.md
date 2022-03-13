# Tackling climate change using spatio-temporal graphs for automated deep learning


## Jupyter notebooks inside docker containers

Download this repository to home directory:
```
cd
git clone https://github.com/ArsamAryandoust/SpatioTemporalGraphs
cd SpatioTemporalGraphs
```

Build Jupyter notebook container:
``` 
docker build -t main_notebook DockerNotebook
```

Compute using CPU with:
``` 
docker run -it -v ~/SpatioTemporalGraphs:/SpatioTemporalGraphs -p 3333:1111 main_notebook
```

Compute using GPUs with:
``` 
docker run -it --gpus all -v ~/SpatioTemporalGraphs:/SpatioTemporalGraphs -p 3333:1111 main_notebook
```


