Kubernetes Cluster setup on AWS with front & backend Staage-1
1. Declarative POD deployment Stage-2
2. Define REPLICASET to maintain the autoscaling Stage-3
3. Define DEPLOYMENT to implement including the REPLICASET Stage-4 : Created Cluster along with NodeGroup
4. Added EBS driver
5. Mapped role with NodeGroup to manage EBS volume a) kubectl apply -k "github.com/kubernetes-sigs/aws-ebs-csi-driver/deploy/kubernetes/overlays/stable/?ref=master"
6. Enabled Kye-Pair for Nodegroup access Frontend & Backend highlights:
7. Claim EBS volume for persistent storage
8. Configmap for DB config script
9. BASE64 encrypted password used
10. Exposed Service on ClusterIP
11. Liveness / Readiness Probe to check the app health
12. Resource allocation
Same can be deployed in multiple NameSpaces

