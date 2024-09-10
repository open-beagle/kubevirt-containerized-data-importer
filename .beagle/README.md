# kubevirt

<https://github.com/kubevirt/containerized-data-importer>

```bash
git remote add upstream git@github.com:kubevirt/containerized-data-importer.git

git fetch upstream

git merge v1.60.2
```

## images

```bash
docker pull quay.io/kubevirt/cdi-operator:v1.60.2 && \
docker tag quay.io/kubevirt/cdi-operator:v1.60.2 registry.cn-qingdao.aliyuncs.com/wod/kubevirt-cdi-operator:v1.60.2 && \
docker push registry.cn-qingdao.aliyuncs.com/wod/kubevirt-cdi-operator:v1.60.2

docker pull quay.io/kubevirt/cdi-controller:v1.60.2 && \
docker tag quay.io/kubevirt/cdi-controller:v1.60.2 registry.cn-qingdao.aliyuncs.com/wod/kubevirt-cdi-controller:v1.60.2 && \
docker push registry.cn-qingdao.aliyuncs.com/wod/kubevirt-cdi-controller:v1.60.2

docker pull quay.io/kubevirt/cdi-importer:v1.60.2 && \
docker tag quay.io/kubevirt/cdi-importer:v1.60.2 registry.cn-qingdao.aliyuncs.com/wod/kubevirt-cdi-importer:v1.60.2 && \
docker push registry.cn-qingdao.aliyuncs.com/wod/kubevirt-cdi-importer:v1.60.2

docker pull quay.io/kubevirt/cdi-cloner:v1.60.2 && \
docker tag quay.io/kubevirt/cdi-cloner:v1.60.2 registry.cn-qingdao.aliyuncs.com/wod/kubevirt-cdi-cloner:v1.60.2 && \
docker push registry.cn-qingdao.aliyuncs.com/wod/kubevirt-cdi-cloner:v1.60.2

docker pull quay.io/kubevirt/cdi-importer:v1.60.2 && \
docker tag quay.io/kubevirt/cdi-importer:v1.60.2 registry.cn-qingdao.aliyuncs.com/wod/kubevirt-cdi-importer:v1.60.2 && \
docker push registry.cn-qingdao.aliyuncs.com/wod/kubevirt-cdi-importer:v1.60.2

docker pull quay.io/kubevirt/cdi-apiserver:v1.60.2 && \
docker tag quay.io/kubevirt/cdi-apiserver:v1.60.2 registry.cn-qingdao.aliyuncs.com/wod/kubevirt-cdi-apiserver:v1.60.2 && \
docker push registry.cn-qingdao.aliyuncs.com/wod/kubevirt-cdi-apiserver:v1.60.2

docker pull quay.io/kubevirt/cdi-uploadserver:v1.60.2 && \
docker tag quay.io/kubevirt/cdi-uploadserver:v1.60.2 registry.cn-qingdao.aliyuncs.com/wod/kubevirt-cdi-uploadserver:v1.60.2 && \
docker push registry.cn-qingdao.aliyuncs.com/wod/kubevirt-cdi-uploadserver:v1.60.2

docker pull quay.io/kubevirt/cdi-uploadproxy:v1.60.2 && \
docker tag quay.io/kubevirt/cdi-uploadproxy:v1.60.2 registry.cn-qingdao.aliyuncs.com/wod/kubevirt-cdi-uploadproxy:v1.60.2 && \
docker push registry.cn-qingdao.aliyuncs.com/wod/kubevirt-cdi-uploadproxy:v1.60.2
```

## install

```bash
kubectl create -f /etc/kubernetes/addons/kubevirt-cdi/kubevirt-cdi-operator.yaml

kubectl create -f /etc/kubernetes/addons/kubevirt-cdi/kubevirt-cdi-cr.yaml
```
