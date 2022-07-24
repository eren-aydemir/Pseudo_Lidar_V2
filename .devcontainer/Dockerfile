# Building on top of nVIDIA Pytorch NGC Container 
FROM nvcr.io/nvidia/pytorch:22.05-py3

# install pycuda
RUN pip3 install pycuda

# install configargparse
RUN pip3 install ConfigArgParse

# install opencv
RUN pip3 install opencv-python

# install scipy
RUN pip3 install scipy

# install imageio
RUN pip3 install imageio

# install tensorboardx
RUN pip3 install tensorboardx

# install tqdm
RUN pip3 install tqdm

# install pillow
RUN pip3 install pillow==6.2.0

# Install Open3D system dependencies and pip
RUN apt-get update && apt-get install --no-install-recommends -y \
    libgl1 \
    libgomp1 \
    python3-pip \
    && rm -rf /var/lib/apt/lists/*

# Install Open3D from the pypi repositories
RUN python3 -m pip install --no-cache-dir --upgrade open3d