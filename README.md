# geoip2-nginx-ingress
Install Nginx Ingress on EKS with features, use Helm to Install:
- Terminate HTTPS traffic on Amazon EKS workloads with ACM
- Use GeoIP2 for block geo country location
- Tunning Nginx Ingress for highload traffic

```
- Get MaxMind Lincese on https://dev.maxmind.com/geoip/geolite2-free-geolocation-data
and input to values `LICENSE_KEY` and  `KXqknCJtN7jd2hir`
- Change annotations `service.beta.kubernetes.io/aws-load-balancer-ssl-cert`
- Install command :
```
```
helm install nginx-ingress ingress-nginx/ingress-nginx --version 4.1.3 -f values.yml
```


![Ingress1](https://user-images.githubusercontent.com/93975934/191185414-92e01667-6754-4a26-a493-a9d0c8d25ade.png)
