# create rbac service account

kubectl apply -f helm-rbac.yaml

# install tiller 

kubectl apply -f tiller.yaml

# install app using helm

helm install --name helm-chatapp .

# delete app using helm

helm del  --purge --name helm-chatapp

