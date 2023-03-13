
Wait for the pods to be ready. It can takes some minutes for the images to be built and deployed.
You can check the status of the pods by calling: `oc get pods -w`.


5. Produces messages

`curl https://$(oc get route jms-producer --template='{{ .spec.host }}')/HelloWorldMDBServletClient`

Check the logs of the mdb-consumer, you will see the traces of the received messages.

