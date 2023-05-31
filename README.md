#Run below command to create EFS-Provisioner


helm install efs-provisioner ./efs-provisioner -f ./efs-provisioner/values.yaml --set efsProvisioner.efsFileSystemId=fs-1234567890 --set efsProvisioner.awsRegion=us-east-2
