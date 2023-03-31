# Deployment Worksheet

__Task 2, step 6: After completing step 5 of task 2, what do you notice about the `ReplicaSet` - what is this used for?__
hint: use ` kubectcl get rs --show-labels`

```
I noticed theres an extra label of pod-template-hash which is used to keep child replica sets of deployments unique.
```

__Task 2, step 7: what command did you use to scale the deployment?__

```
kubectl scale deployment/nginx-deployment --replicas=3
```

__Task 3, step 2: Why are there two replica sets but only one deployment?__

```
The one deployment houses the two distinct replica sets because changing label information after deployment can cause orphaned sets.
```

__Task 3, step 6: What command did you use to roll back the deployment?__

```
kubectl rollout undo deployment nginx-deployment
```
