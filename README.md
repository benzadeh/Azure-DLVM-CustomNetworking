# Azure-DLVM-CustomNetworking
ARM template to create a DLVM Windows machine by using existing Virtual Network 

The Deep Learning Virtual Machine template is a nested template. The first template defines the OS and based on that, it will trigger one of the below templates. 
https://deeplearningvmstg.blob.core.windows.net/assets/WindowsServer2016.json
https://deeplearningvmstg.blob.core.windows.net/assets/UbuntuLinux.json

The original template, creates a Virtual network and Public IP addresses. In this template the Public IP is removed, and you have to specify a Virtual Network and Subnet name. This template uses WindowsServer. 

Follow these steps to deploy the template from the portal: 

1-	Under All Services, search for Template service 

 

2-	Create a new Template and replace the content with the content of WindowsServer2016.json. 
3-	Save and Deploy 
a.	The template asks for information for existing Virtual network. 


