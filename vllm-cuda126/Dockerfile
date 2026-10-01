FROM docker.io/vllm/vllm-openai:latest

USER root

RUN uv pip install torch==2.13.0 --index-url https://download.pytorch.org/whl/cu126

USER vllm
WORKDIR /home/vllm
ENTRYPOINT ["/usr/local/bin/vllm-nonroot-entrypoint.sh"]

