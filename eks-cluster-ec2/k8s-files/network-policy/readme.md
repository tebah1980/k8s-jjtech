k exec -it -n application <name of pod a> -- <curl ip of pod b>

kubectl get clusterrole aws-node -o yaml > tempfile.yaml
cat tempfile.yaml append.yaml | kubectl apply -f -
rm tempfile.yaml
