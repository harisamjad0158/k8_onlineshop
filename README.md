nano cluster.yml

kind create cluster --config cluster.yml --name tws-cluster

kubectl get nodes

kubectl get nodes -w

kubectl apply -f https://kind.sigs.k8s.io/examples/ingress/deploy-ingress-nginx.yaml

kubectl get svc -n ingress-nginx

sudo -E kubectl port-forward -n ingress-nginx svc/ingress-nginx-controller 80:80 --address=0.0.0.0 &

docker login -u johncorner158

docker build -t johncorner158/k8_onlineshop:latest .

docker run -p 81:80 johncorner158/k8_onlineshop:latest

docker push johncorner158/k8_onlineshop:latest

cd k8s

kubectl apply -f a.yml

kubectl get ns

kubectl get pods -n online-shop-prod

kubectl get hpa -n online-shop-prod

kubectl describe hpa online-shop -n online-shop-prod

kubectl port-forward --address 0.0.0.0 svc/online-shop 8080:80 -n online-shop-prod

# browse >>> http://ip:8080/shop

kubectl apply -f a.yml
