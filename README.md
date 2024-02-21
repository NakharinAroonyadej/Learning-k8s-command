# Learning-k8s-command : Store command for using in k8s
 this is the file that i use to memorize all command for using k8s
## create deployment and pod
 kubectl create deployment -n <namespace> --image=<image_name> <deployment_name>
## create service and expose deployment
 kubectl expose deployment -n <namespace> <deployment_name> --port=<k8s_port> --target-port=<program_port> <service_name>
## Change service to nodeport
 - change type from ClusterIP to NodePort
 - add nodePort inside - port and assign to public port
 - map router between nodePort and public port
