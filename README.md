# sagemaker-model-training

Avant de build la premiere fois -> authentification sur aws et pull l'image.

$(aws ecr get-login --profile 952897906699 --region eu-west-1 --no-include-email --registry-ids 763104351884)
docker pull 763104351884.dkr.ecr.eu-west-1.amazonaws.com/tensorflow-training:1.14-cpu-py3

ensuite :

docker build -t nom-du-container project/

