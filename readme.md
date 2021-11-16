# Solution 

## How to deploy the dummy controller 

To deploy the dummy controller you need to run the following command : 

```bash
$ make deploy IMG=ayoubensalem/dummy-controller:v1
```

This will deploy the controller on the namespace : `tmp-homework-ae-system`


## Create a dummy object 

To create a dummy object, run the following command : 

```bash
$ kubectl create -f config/samples/_v1alpha1_dummy.yaml
```

You can check the logs of the controller by running : 

```bash
$ kubectl logs -f deploy/tmp-homework-ae-controller-manager -n tmp-homework-ae-system -c manager
```
