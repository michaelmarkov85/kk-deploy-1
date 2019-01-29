In order to FluentD to scrape logs from node's pods node must be labeled with
nodeSelector:
    beta.kubernetes.io/fluentd-ds-ready: "true"
run 
kubectl label nodes NODE_NAME_HERE beta.kubernetes.io/fluentd-ds-ready=true
