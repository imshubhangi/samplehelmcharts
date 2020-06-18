# samplehelmcharts
helm repo add samplehelmcharts https://imshubhangi.github.io/samplehelmcharts
 
helm repo list
 
 cat > /tmp/values.yaml
env:
  count: one
 
helm install mychart samplehelmcharts/chart -f /tmp/values.yaml
 
kubectl get pods ; kubectl get deployments
 

kubectl exec <podname> cat  /var/www/html/webpage.html
