# Tackling climate change using automated deep learning with spatio-temporal event graphs

We are building an intelligent pipeline from reading raw data to fully analyzing the data in every possible shape and form based on both the passed (potentially private) data and any publicly available data. For this purpose, we are using the flexibility of neural networks for deep learning and combine it with a spatio-temporal event graph model. We use this spatio-temporal graph representation of our data to derive a standardized way of deriving computations graphs using the concept graph neural networks.


<img src="figures/drawing.png" alt="blueprint" title="Overview blueprint">



Download this repository to your home directory:
```
cd
git clone https://github.com/ArsamAryandoust/SpatioTemporalGraphs
cd SpatioTemporalGraphs
```

## Docker

Build main:
``` 
docker build -t main Docker
```

## Jupyter notebooks inside docker containers

Build Jupyter notebook container:
``` 
docker build -t main_notebook DockerNotebook
```

Compute using CPU only:
``` 
docker run -it -v ~/SpatioTemporalGraphs:/SpatioTemporalGraphs -p 3333:1111 main_notebook
```

Compute using GPUs too:
``` 
docker run -it --gpus all -v ~/SpatioTemporalGraphs:/SpatioTemporalGraphs -p 3333:1111 main_notebook
```


