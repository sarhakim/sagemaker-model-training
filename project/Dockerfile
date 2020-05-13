FROM 763104351884.dkr.ecr.eu-west-1.amazonaws.com/tensorflow-training:2.0-cpu-py3
LABEL maintainer=""

WORKDIR /workspace
COPY requirements.txt .
RUN pip install --no-cache-dir -U -r requirements.txt
COPY main.py .
COPY scripts/ scripts/
COPY tests/ tests/

ENTRYPOINT ["python", "main.py"]
CMD ["train"]
