# azure_kubernetes_service
some doc for azure kubernetes service
-Docker
  �n�Jcontainer registry
  ```
  az acr login --name mygistry
  ```
  �άO
  ```
  docker login myregistry.azurecr.io -u xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx -p myPassword
  ```
  
  �b�N�M�����e�ܱz���n�����e�A�����ϥ� ACR �n�J���A���W�٨ӼаO�M���C �ϥ� docker tag �R�O�ӼаO�M���C �N�n�J���A�����N���z���e�O�����n�J���A���W�١C
  ```
  docker tag <image repository name> <login server>/<image name>:<version>
  ```
  
  �̫��image���e�Wcontainer registry
  ```
  docker push <login server>/aci-helloworld:v1
  ```
  