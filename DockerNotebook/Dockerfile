FROM pytorch/pytorch:latest

RUN pip3 install jupyter

WORKDIR /SpatioTemporalGraphs
CMD jupyter notebook --ip 0.0.0.0 --port 1111 --no-browser --allow-root
