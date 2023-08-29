{
  "code": "DeploymentFailed",
  "target": "/subscriptions/481a005a-d39d-49ea-8b74-da1ffe9a12d4/resourceGroups/genshimage/providers/Microsoft.Resources/deployments/CreateVm-genshappvm-image-20230829185804-20230829190909",
  "message": "At least one resource deployment operation failed. Please list deployment operations for details. Please see https://aka.ms/arm-deployment-operations for usage details.",
  "details": [
    {
      "code": "ResourceDeploymentFailure",
      "target": "/subscriptions/481a005a-d39d-49ea-8b74-da1ffe9a12d4/resourceGroups/genshimage/providers/Microsoft.Compute/virtualMachines/lastvm",
      "message": "The resource write operation failed to complete successfully, because it reached terminal provisioning state 'Failed'."
    }
  ]
}


{
  "code": "DeploymentFailed",
  "target": "/subscriptions/481a005a-d39d-49ea-8b74-da1ffe9a12d4/resourceGroups/genshimage/providers/Microsoft.Resources/deployments/CreateVm-genshweb-v2.3.1-29-08-2023-20230829182725",
  "message": "At least one resource deployment operation failed. Please list deployment operations for details. Please see https://aka.ms/arm-deployment-operations for usage details.",
  "details": [
    {
      "code": "ResourceDeploymentFailure",
      "target": "/subscriptions/481a005a-d39d-49ea-8b74-da1ffe9a12d4/resourceGroups/genshimage/providers/Microsoft.Compute/virtualMachines/testwebvm",
      "message": "The resource write operation failed to complete successfully, because it reached terminal provisioning state 'Failed'."
    }
  ]
}


{
  "code": "DeploymentFailed",
  "target": "/subscriptions/481a005a-d39d-49ea-8b74-da1ffe9a12d4/resourceGroups/genshimage/providers/Microsoft.Resources/deployments/CreateVm-shadow-web-v2.3.1-29-08-2023-20230829170443",
  "message": "At least one resource deployment operation failed. Please list deployment operations for details. Please see https://aka.ms/arm-deployment-operations for usage details.",
  "details": [
    {
      "code": "ResourceDeploymentFailure",
      "target": "/subscriptions/481a005a-d39d-49ea-8b74-da1ffe9a12d4/resourceGroups/genshimage/providers/Microsoft.Compute/virtualMachines/testwenserver",
      "message": "The resource write operation failed to complete successfully, because it reached terminal provisioning state 'Failed'."
    }
  ]
}

Issue resolve hua while creation of vm from the image in the different vnet from where the existing vm was backed up.
