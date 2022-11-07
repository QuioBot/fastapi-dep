export KUBECONFIG=/Users/omarelghiba/Desktop/Project/Digital_Marketing_APi/.kube/kubeconfig.yaml

kubectl create secret generic django-web-env-prod  --from-env-file=web/.env.prod

docker buildx build --platform=linux/amd64 -t registry.digitalocean.com/om-k8s/django-k8s-web:latest -f Dockerfile .

docker push registry.digitalocean.com/om-k8s/django-k8s-web --all-tags



kubectl apply -f k8s/apps/django-k8s-web.yaml
kubectl delete -f k8s/apps/django-k8s-web.yaml
kubectl get deployments
kubectl get services
kubectl get nodes
kubectl get pods
kubectl exec -it <podname> -- /bin/bash
kubectl get services <service name> -0 yaml


docker login registry.digitalocean.com

token : dop_v1_f0279ab45a6cb080858b5de321ee167bde873a80ddac5f000f09bcd6af5211fb

docker buildx build --platform=linux/amd64 -t registry.digitalocean.com/quiobot-cnt/django-k8s-web:latest -f Dockerfile .

docker push registry.digitalocean.com/quiobot-cnt/django-k8s-web --all-tags


python -c "import secrets:print(secrets.token_urlsafe(32))"

kubectl get secrets

kubectl create secret generic django-k8s-web-prod-env --from-env-file=web/.env.prod

kubectl get secret  django-k8s-web-prod-env -o YAML

kubectl delete secret  django-k8s-web-prod-env

kubectl get pods -w


echo "# QuioBot-Chatbot" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/QuioBot/QuioBot-Chatbot.git
git push -u origin main


git remote add origin https://github.com/QuioBot/QuioBot-Chatbot.git
git branch -M main
git push -u origin main


action token : dop_v1_c72ac5455ba0e4c8ef45d6648e8132f0e83d541fd4ccea255c83bc3d8c62be64


git remote remove origin  

doctl auth init

doctl token dop_v1_97548bbc102389a9523dd5da2914c2aeae149ae4482af96b38c084e75d9a4065


doctl registry kubernetes-manifest | kubectl apply -f -



docker github action token : dckr_pat_eU5MjMz1vfeEk1KLJTIg2U56yBU

