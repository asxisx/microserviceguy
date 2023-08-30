# Error at Azure Advisor (under Reliability)

Virtual Machines in your subscription are running on images that have been scheduled for deprecation. Once the image is deprecated, new VMs cannot be created from the deprecated image. Upgrade to newer SKU of the image to prevent disruption to your workloads.
Upgrade your VM to alternative image plan


https://aka.ms/DeprecatedImagesFAQ

# Solution

-  We can use that same deprecated image by first we need to make a custom image of that vm. Probably by making one recovery vm from the running vm snapshot.
-  Create a new vm under the same host pool, only possible if the current vm doesn't have the data.
