# azure_kubernetes_service

## Docker
  �n�J container registry
  ```cmd
  az acr login --name mygistry
  ```
  �άO
  ```cmd
  docker login myregistry.azurecr.io -u xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx -p myPassword
  ```
  
  �b�N�M�����e�ܱz���n�����e�A�����ϥ� ACR �n�J���A���W�٨ӼаO�M���C �ϥ� docker tag �R�O�ӼаO�M���C �N�n�J���A�����N���z���e�O�����n�J���A���W�١C
  ```cmd
  docker tag <image repository name> <login server>/<image name>:<version>
  ```
  
  ��§�image ���Wdockerhub
  ```cmd
  docker push <username>/<repo name>:<Tag name>
  ```
  �̫��image���e�Wcontainer registry
  ```cmd
  docker push <login server>/<repo name>:<Tag name>
  ```
  