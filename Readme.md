	•	Project Steps:
    •	Build the app locally.
    •	Add Jenkinsfile, Dockerfile, deployment.yaml and service.yaml.
    •	Push it to GitHub Repository by Git.
    •	Triggered Jenkins Server to start the Pipeline by Webhook.
    •	The stages: 
      ⁃	Increment the version app.
      ⁃	Build maven app.
      ⁃	Build Docker image and Push to ECR.
      ⁃	Deploy the App on EKS after Pulling the image from ECR.
      ⁃	Commit the changes (app version) to GitHub Repository.

————————————
	•	AWS:
    ⁃	Create account with MFA.
    ⁃	Lunch EC2 instance and install Jenkins on it.
    ⁃	Create ECR Repo.
    ⁃	Create VPC by CloudFormation and IAM roles for EKS Cluster.
    ⁃	Create EKS Cluster + Node Group with 2 nodes.
————————————
	•	Jenkins Server:
    ⁃	Install Kubectl.
    ⁃	Install aws-iam-authenticator.
    ⁃	Install Kubeconfig Manually.
    ⁃	Add credentials for ECR and AWS Account (access-key, secret-access-key).
————————————
	•	Kubernetes:
    ⁃	Create deployment.yaml for java-maven-app.
    ⁃	Create service.yaml for deployment.
    ⁃	Create secret directly in the cluster to be able to pull the image from ECR.

————————————
————————————

The Project is done…
