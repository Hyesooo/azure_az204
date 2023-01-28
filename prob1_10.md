### 💯 prob1 ~ 11

1. 두개의 Hiper-v 호스트가 있다. Host1은 VM1에 디플로이 되어있는데, 이를 Host2d-에 옮기기 위해 할 일은?     
🔔 **From th Redeploy blade, click Redelploy**
   > 💡 Hiper-v ? 윈도우 가상화 프로그램.
   > 새 호스트로 바꾸고 싶은 경우 재 배포할 것.

2. 디플로이를 위해 ARM tamplate을 다운로드 받았다. 그러나 비번이 palin-text이기떄문에, administrative password 참조를 적용해야한다. 이 때 할 일은?      
🔔 **Azure key valut, Access policy**
   > 💡 Using an Access Policy we allow access to the previously created secret.
   
3. AAD에 joined된 AKS를 관리 중일 때, 개발자가 myApp을 여기에 배포하고자 한다. 이 앱을 위해 YML 매니패스트 파일을 deployee해야하는데, 알맞은 액션은?  
🔔 **Azure CLI를 로컬에 설치 후 run the kubectl apply f myapp.yaml command**
   > To deploy a YAML file to Kubernetes you need to use the “kubectl” command 

4.  same with no.3
5. 새로운 데이터가 큐에 들어올때마다 코드의 특정 함수를 인보크 시키는 앱 서비스의 백그라운드 태스크를 트리거 하도록 디자인 된 WebJobs SDK 사용할때, 큐 아이템들을 처리하는 서비스 구성을 하려고한다. 이떄 사용할 서비스는?  
🔔 **WebJobs**  
   > 특별한 언급이 없다면 WebJobs SDK와 가장 호환이 좋은것은 webJobs, 그러나 Function과 비교했을 때 기능이 안되는 것이 많음.


