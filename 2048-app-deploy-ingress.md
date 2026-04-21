#Create Fargate profile
eksctl create fargateprofile \
    --cluster demo-cluster \
    --region us-east-1 \
    --name alb-sample-app \
    --namespace game-2048

#Deploy the deployment, service and Ingress


kubectl apply -f https://raw.githubusercontent.com/kubernetes-sigs/aws-load-balancer-controller/v2.5.4/docs/examples/2048/2048_full.yaml
<img width="813" height="757" alt="image" src="https://github.com/user-attachments/assets/517a17bb-ed0e-414d-8578-ad38e72d49d1" />
