# azure_kubernetes_service
some doc for azure kubernetes service
-Docker
  登入container registry
  ```
  az acr login --name mygistry
  ```
  或是
  ```
  docker login myregistry.azurecr.io -u xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx -p myPassword
  ```
  
  在將映像推送至您的登錄之前，必須使用 ACR 登入伺服器名稱來標記映像。 使用 docker tag 命令來標記映像。 將登入伺服器取代為您先前記錄的登入伺服器名稱。
  ```
  docker tag <image repository name> <login server>/<image name>:<version>
  ```
  
  最後把image推送上container registry
  ```
  docker push <login server>/aci-helloworld:v1
  ```
  