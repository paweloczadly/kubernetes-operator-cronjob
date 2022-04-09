# kubernetes-operator-cronjob

Kubernetes operator which creates CronJobs. Based on: https://book.kubebuilder.io/cronjob-tutorial/cronjob-tutorial.html

## Usage

1. Setup Kubernetes cluster locally:

```
$ minikube start
```

2. Install CRDs into the cluster:

```
$ make install
```

3. Run the operator:

```
$ make run
```

4. In the new terminal tab deploy the sample CronJob:

```
$ kubectl apply -f config/samples/
```

5. Verify if the CronJob has been created:

```
$ kubectl get cronjobs.batch.paweloczadly.io
$ kubectl get jobs
```
