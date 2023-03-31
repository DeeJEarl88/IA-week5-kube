# ReplicaSet Worksheet:

__Task 1, step 7: Enter the command you used for scaling the replica set:__
```
kubectl scale --replicas=3 rs/nginx-replica
```

__Task 1, step 9: What happened after applying another pod with matching selectors as the ReplicaSet?__
```
I see an additional pod when created and immediately deleted.
The ReplicaSet matched the new pods due to labels and shut it down.
```
