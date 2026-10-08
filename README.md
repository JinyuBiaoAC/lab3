# lab3

# demo link

https://youtu.be/Pk_HwHKEcoA

# repos

-https://github.com/JinyuBiaoAC/cst8915lab2_RabbitMQ
-https://github.com/JinyuBiaoAC/lab3_store_front
-https://github.com/JinyuBiaoAC/lab3_product_service
-https://github.com/JinyuBiaoAC/lab3_order_service

# reflection questions

## The challenges I encountered was : 
1. could not deploy static web app due to regional restriction.
2. <img width="432" height="321" alt="order service authentication error" src="https://github.com/user-attachments/assets/445f6f02-7103-487a-90c4-6b236b21c58f" /> failed to assign user-assigned identity to order service (fixed with reusing the identity for product service)
3. failed to place order due to a mistake when setting up the environment variable in the order service app

## How does deploying microservices on Azure Web App Service differ from running them locally?
The differences I noticed was that first it provides a managed hosting environment, so I do not need to manually manage the deployment or install the dependencies such as requirement.txt, instead, azure will do them for me. What I needed to do was to tell Azure which dependencies are needed. Azure also provides the public url for me so I do not need to use the url of the virtual machine. The service also constantly running without executing the command to run it, unless I stop the service on my own.

## Why is it important to use environment variables for configurations in a cloud environment?
It is important because they keep the configuration separate from the code. Whenever I need to change the environments I just need to go to Azure to change it. It also helps on data security since the sensitive information such as account name and password do not need to be stored in the git repository.
