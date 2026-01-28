## Command to bind a loadbalancer to istio-ingressgateway service

 kubectl patch svc istio-ingressgateway -n istio-system \
  -p '{
    "metadata": {
      "annotations": {
        "kubernetes.io/elb.id": "43055bd0-a198-4ed8-ba77-5b7dd1b8395f",
        "kubernetes.io/elb.class": "union",
        "kubernetes.io/elb.lb-algorithm": "ROUND_ROBIN"
      }
    }
  }'


  # Reference 
  Istio on Huawei cloud https://istio.io/latest/es/docs/setup/platform-setup/huaweicloud/ 
