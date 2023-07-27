FROM paddlepaddle/paddle:2.4.2-gpu-cuda11.7-cudnn8.4-trt8.4
ARG DEBIAN_FRONTEND=noninteractive
RUN echo 'start build'
RUN LC_ALL=C.UTF-8
RUN apt update && apt install git -y
RUN pip3 install jupyter_echarts --user -i https://mirrors.ustc.edu.cn/pypi/web/simple
RUN pip3 install pipenv --user -i https://mirrors.ustc.edu.cn/pypi/web/simple
ENV PATH="$PATH:/root/.local/bin"
ENTRYPOINT tail -f /dev/null