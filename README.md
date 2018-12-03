# golang_eos
eos build env based on golang

#create the image 
docker build -t eos_golang:latest .

#run into docker to build chain33 pro
docker run -it --rm -v ~/go/src/gitlab.33.cn/chain33/chain33:/go/src/gitlab.33.cn/chain33/chain33 eos_golang /bin/bash
