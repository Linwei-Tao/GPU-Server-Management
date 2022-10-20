# How to use multiple gpus most efficiently?

In our lab, we have three 4*4090 servers shared between 10 members. 

In order to take the most use of GPU resources. 

1. We use `NFS` system to store our code and model weights only one copy on a file server (this can be any server that has a large disk). 
2. Then, we mount the file folder to each gpu server and get access to these files.
3. We store all datasets on each server, which make it much faster to read the dataset locally.
4. We use `Pycharm SSH Interpreter` to get access to the python interpreter of each node and run code in the mounted files.
5. In order to get the gpu usage info, we build a [GPU monitoring dashboard](https://github.com/Linwei-Tao/GPU-Server-Management/blob/main/monitor_gpuinfo.md) to show the current gpu usage info.
