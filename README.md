## A resume of PROMPTS
---
###  

- Generated with kubectl-ai
- Model used: gemini-2.5-pro 

## General information:

| NAME | PROMPT | DESCRIPTION | EXAMPLE |
|---|---|---|---|
| app.yaml | Create a Kubernetes Pod named app with the label "app: demo", running the gcr.io/k8s-k3s/demo:v1.0.0 image and exposing port 8000. | App deployment example | [app.yaml](https://github.com/git-account/demo/blob/bf62404d921f8ee3e343c85de89dbc23152640e4/yaml/app.yaml) |
| app-livenessProbe.yaml | Create a Kubernetes Pod named "app-livenessprob" in the demo namespace, running the gcr.io/k8s-k3s/demo:v1.0.0 image with an HTTP liveness probe checking the / path on port 8000. | LivenessProbe example | [app-livenessProbe.yaml](https://github.com/git-account/demo/blob/bf62404d921f8ee3e343c85de89dbc23152640e4/yaml/app-livenessProbe.yaml) |
| app-readinessProbe.yaml | Create a Kubernetes Pod named "app-readinessprob" with a gcr.io/k8s-k3s/demo:v2.0.0 image, a liveness probe on the  /  path, and a readiness probe checking the /ready  path on port 8000. | ReadinessProbe example | [app-readinessProbe.yaml](https://github.com/git-account/demo/blob/bf62404d921f8ee3e343c85de89dbc23152640e4/yaml/app-readinessProbe.yaml) |
| app-volumeMounts.yaml | Create a Kubernetes Pod named "app-volume" running the  gcr.io/kuar-demo/kuard-amd64:1 image, which mounts the host's /var/lib/app directory to the /data path inside the container and includes liveness and readiness probes. | Mount path example | [app-volumeMounts.yaml](https://github.com/git-account/demo/blob/bf62404d921f8ee3e343c85de89dbc23152640e4/yaml/app-volumeMounts.yaml)|
| app-cronjob.yaml | Create a Kubernetes CronJob named "app-cronjob" that runs a bash container every five minutes to print 'Hello world'.| Cronjob example | [app-cronjob.yaml](https://github.com/git-account/demo/blob/bf62404d921f8ee3e343c85de89dbc23152640e4/yaml/app-cronjob.yaml) |
| app-job.yaml | Create a Kubernetes Job named "app-job-rsync" that uses the Google Cloud SDK image to rsync data from a GCS bucket to a GCE persistent disk mounted in the container. | Rsync example | [app-job.yaml](https://github.com/git-account/demo/blob/bf62404d921f8ee3e343c85de89dbc23152640e4/yaml/app-job.yaml)|
| app-multicontainer.yaml | Create a multi-container Pod named "app-multi-containers" where a Debian container continuously writes the date to a shared volume, and an Nginx container serves that content. | Multicontainer pod example | [app-multicontainer.yaml](https://github.com/git-account/demo/blob/bf62404d921f8ee3e343c85de89dbc23152640e4/yaml/app-multicontainer.yaml) |
| app-resources.yaml | Create a Kubernetes Pod named "app-resource" with liveness and readiness probes, and set CPU/memory resource requests to '100m'/'128Mi' and limits to '100m'/'256Mi'.". | Resource limiting example | [app-resources.yaml](https://github.com/git-account/demo/blob/bf62404d921f8ee3e343c85de89dbc23152640e4/yaml/app-resources.yaml) |

