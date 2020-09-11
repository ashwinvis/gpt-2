# How to get started

## Requirements

- docker
- nvidia-container-runtime (AUR) - Did not work, in ArchLinux.
- ~20 GB of disk space

## Installation

```{.sh}
ln -s Dockerfile.gpu Dockerfile
sudo -u docker docker build . -t gpt-2
```

## Running

```{.sh}
# docker run -p 8888:8888 --runtime=nvidia gpt-2
```

# Alternatively

## Native Installation

- tensorflow-cuda
- python-tensorflow-cuda
- See requirements-2020-09-11.txt for other python requirements and versions


Download the models:

```{.sh}
python3 download_model.py 124M
python3 download_model.py 355M
python3 download_model.py 774M
python3 download_model.py 1558M
```
