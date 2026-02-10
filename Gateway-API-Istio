## Command to bind a loadbalancer to gateway-api-istio service

kubectl patch svc gateway-api-istio -n default -p '{
  "spec": {
    "ipFamilyPolicy": "SingleStack",
    "ipFamilies": ["IPv4"]
  },
  "metadata": {
    "annotations": {
      "kubernetes.io/elb.id": "aaf5d552-5f0d-4ee2-9b15-31d8f2a26342",
      "kubernetes.io/elb.class": "union",
      "kubernetes.io/elb.lb-algorithm": "ROUND_ROBIN"
    }
  }
}'



