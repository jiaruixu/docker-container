FROM tensorflow/tensorflow:1.10.0-devel-gpu-py3

RUN apt-get update && \
    apt-get install -y python3-pip git
RUN pip3 install numpy scipy moviepy Pillow && \
    pip3 install lmdb opencv-python cryptography h5py six glob

RUN cd /root && git clone https://github.com/hardikbansal/Fader-Networks-Tensorflow.git && \
    cd Fader-Networks-Tensorflow && \
    git checkout 22cc9bd2c76737a28c51d9965639fad176910066

WORKDIR /root/Fader-Networks-Tensorflow
