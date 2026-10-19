# Nginx webserver sample deployment

- testing Horizontal Pod Autoscaler functionality
  - replica count varies from 2 to 5
  - scaling out happens on +80% of CPU average utilization
  - use `siege` on master-node guest (or locally on host) to run stress tests and trigger autoscaler

- includes resource:
  - Deployment
  - Service
  - Horizontal Pod Autoscaler (HPA)

- used for playground in [sample-k8s-gitops](https://github.com/gek0/sample-k8s-gitops) repository
- namespace created with ArgoCDs
