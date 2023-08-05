#Run below command to create EFS-Provisioner


change storageclass apiVersion in file templates/storageclass.yaml from apiVersion: storage.k8s.io/v1beta1 to apiVersion: storage.k8s.io/v1


helm install efs-provisioner ./efs-provisioner -f ./efs-provisioner/values.yaml --set efsProvisioner.efsFileSystemId=fs-1234567890 --set efsProvisioner.awsRegion=us-east-2


PodSecurityPolicy is deprecated in v1.21+, unavailable in v1.25+  . So podsecuritypolicy.yaml file has been deleted.
