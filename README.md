# azure_kubernetes_service

## Docker
  登入 container registry
  ```cmd
  az acr login --name mygistry
  ```
  或是
  ```cmd
  docker login myregistry.azurecr.io -u xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx -p myPassword
  ```
  
  在將映像推送至您的登錄之前，必須使用 ACR 登入伺服器名稱來標記映像。 使用 docker tag 命令來標記映像。 將登入伺服器取代為您先前記錄的登入伺服器名稱。
  ```cmd
  docker tag <image repository name> <login server>/<image name>:<version>
  ```
  
  單純把image 推上dockerhub
  ```cmd
  docker push <username>/<repo name>:<Tag name>
  ```
  最後把image推送上container registry
  ```cmd
  docker push <login server>/<repo name>:<Tag name>
  ```
  