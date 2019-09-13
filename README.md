# Helm Examples

## Playing with Helm and Helm Chart to deploy a simple image (Alpine Linux) which sleeps (donothing)

createPod.yaml was a reverse-engineering to deploy (directly) with the command:

[Code] $ kubectl create -f createPod.yaml    

the above command, not Helm related at all, but direct interaction with K8S.

the Alpine directory contains the logical structure, and templates\deployment.yaml contains working YAML
with the values and Chart.yaml substitutions for the Alpine Chart

Contrasting the two, you can distill the necessary elements for a simple deployment.

This is done, as to understand what is passed to the K8S API, in we may directly call the REST API,
or leverage one of the K8S client libraries (like the Go Client Library for K8S)
