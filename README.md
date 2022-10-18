# TalkNet patching test fork
This fork was made mostly to test patching weird issues I get when running docker on my machine (Ryzen 5900X, 64GB DDR4-3200, 5700XT for main GPU and a 1050ti for audio CUDA), might pull in additions from other forks such as different voice sets as time goes on and my need for dumber and dumber content ideas arise.

## Requirements
* A Google account to run Colab, or...
* An NVIDIA GPU with 4+ GB of VRAM
* 10 GB of free space

## How to run
### Google Colab
* [Go to the Colab notebook](https://colab.research.google.com/drive/1aj6Jk8cpRw7SsN3JSYCv57CrR6s0gYPB) and follow the instructions.

### TalkNet Offline (Windows)
Fugouddaheah

### Docker (Linux)
* Install Docker and NVIDIA Container Toolkit.
* [Download the Dockerfile.](https://raw.githubusercontent.com/SortAnon/ControllableTalkNet/main/Dockerfile)
Open a terminal, and navigate to the directory where you saved it.
* Run ```docker build -t talknet-offline .``` to build the image. Add ```sudo``` if you're not using rootless Docker.
* Run ```docker run -it --gpus all -p 8050:8050 talknet-offline``` to start TalkNet on http://127.0.0.1:8050/.
