### 💯 prob1 ~ prob11

1. 두개의 Hiper-v 호스트가 있다. Host1은 VM1에 디플로이 되어있는데, 이를 Host2d-에 옮기기 위해 할 일은?     
🔔 **From th Redeploy blade, click Redelploy**
   > 💡 Hiper-v ? 윈도우 가상화 프로그램.
   > 새 호스트로 바꾸고 싶은 경우 재 배포할 것.

2. 디플로이를 위해 ARM tamplate을 다운로드 받았다. 그러나 비번이 palin-text이기떄문에, administrative password 참조를 적용해야한다. 이 때 할 일은?      
🔔 **Azure key valut, Access policy**
   > 💡 Using an Access Policy we allow access to the previously created secret.
   
3. AAD 조인된 AKS로 서비스할 때, 컨테이너 이미지에 패키징된 app의 YAML 매니패스트 파일을 디플로이 하기 위해서 Azure CLI에서 돌릴 명령어?  
   🔔 **kubectl apply -f myapp.yaml**
   > 💡 docker run -it microsoft/azure-cli:0.10.17 " it's a Docker command, not a K8's command.
4. 