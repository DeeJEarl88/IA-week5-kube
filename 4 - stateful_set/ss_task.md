# StatefulSet Worksheet

__Task 5, step 3: Describe what happened and what you noticed about the pods and the volumes for them.__

```
The stateful controller managed created 3 pods and their corresponding volume claims.
```

__Task 5, step 4: Did anything change? Why or why not?__

```
Nothing changed because changes apply when an item is deleted
```

__Task 5, step 6: What happened and why?__

```
A new pod was created in it's place but with version 2.0 because the stateful controller must maintain replicas.
```

__Task 5, step 9: What happens this time?__

```
This time the updates were rolled across the existing instances and all where updated to version 3.0
```

__Task 5, step 11: Repeat step 10. Was everything deleted? Why or why not?__

```
No. Persistent volumes claims default behavior is Retain. 
```