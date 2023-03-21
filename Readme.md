###Project Steps:
	1.Build the app locally.
	2.Add Jenkinsfile, Dockerfile, deployment.yaml and service.yaml.
	3.Push it to GitHub Repository by Git.
	4.Triggered Jenkins Server to start the Pipeline by Webhook.
	5.The stages: 
		a.Increment the version app.
		b.Build maven app.
		c.Build Docker image and Push to ECR.
		d.Deploy the App on EKS after Pulling the image from ECR.
		e.Commit the changes (app version) to GitHub Repository.


###AWS:
1.Create account with MFA.
2.Lunch EC2 instance and install Jenkins on it.
3.Create ECR Repo.
4.Create VPC by CloudFormation and IAM roles for EKS Cluster.
5.Create EKS Cluster + Node Group with 2 nodes.


###Jenkins Server:
	1.Install Kubectl.
	2.Install aws-iam-authenticator.
	3.Install Kubeconfig Manually.
	4.Add credentials for ECR and AWS Account (access-key, secret-access-key).




###Kubernetes:
	1.Create deployment.yaml for java-maven-app.
	2.Create service.yaml for deployment.
	3.Create secret directly in the cluster to be able to pull the image from ECR.



The Project is done…
