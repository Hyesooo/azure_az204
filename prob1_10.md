### 💯 prob1 ~ prob11

1. 두개의 Hiper-v 호스트가 있다. Host1은 VM1에 디플로이 되어있는데, 이를 Host2d-에 옮기기 위해 할 일은?     
🔔 **From th Redeploy blade, click Redelploy**
   > :black_nib: Hiper-v ? 윈도우 가상화 프로그램.
   > 새 호스트로 바꾸고 싶은 경우 재 배포할 것.

2. 디플로이를 위해 ARM tamplate을 다운로드 받았다. 그러나 비번이 palin-text이기떄문에, administrative password 참조를 적용해야한다. 이 때 할 일은?      
🔔 **Azure key valut, Access policy**
   > :black_nib: Using an Access Policy we allow access to the previously created secret.
3. AAD에 joined된 AKS를 관리 중일 때, 개발자가 myApp을 여기에 배포하고자 한다. 이 앱을 위해 YML 매니패스트 파일을 deployee해야하는데, 알맞은 액션은?  
🔔 **Azure CLI를 로컬에 설치 후 run the kubectl apply f myapp.yaml command**
   > :black_nib: To deploy a YAML file to Kubernetes you need to use the “kubectl” command 

4.  *same with no.3*  
   </br>
5. 새로운 데이터가 큐에 들어올때마다 코드의 특정 함수를 인보크 시키는 앱 서비스의 백그라운드 태스크를 트리거 하도록 디자인 된 WebJobs SDK 사용할때, 큐 아이템들을 처리하는 서비스 구성을 하려고한다. 이떄 사용할 서비스는?  
🔔 **WebJobs**  
   > :black_nib: 특별한 언급이 없다면 WebJobs SDK와 가장 호환이 좋은것은 webJobs, 그러나 Function과 비교했을 때 기능이 안되는 것이 많음.
   
6. ARM 탬플릿으로 애저 리소스를 디플로이 하고자 한다. VM은 하나의 가용성 집합을 갖고 있다. ARM 탬플릿이 장애 또는 유지보수시에 가능한 많은 VM에 접근가능하게 유지하고 싶다. platformFaultDomainCount에 어떤 설정을 할것인가?   
   🔔 **Max Value**  
   > :black_nib: Max value for Fault Domain is 3 and Update Domain is 20 in a single availablity set.

7.  *same with no.6*  
   </br>
8.  CosmosDB SQL API 이용하는데, Iot 디바이스에 정보가 들어오면 이메일알림을 보내야한다. (비용 절감도 체크해야함.) 알맞은 funtion App 설정은?     
   🔔 **consumption plan, sendGrid binding**     
      > :black_nib: 비용절감위해 comsumtion plan 체크하고, 애저 펑션에서 이메일 보내기 위해서는 sendGrid 바인딩을 이용한다. sendGrid API는 azure에서 사용하는 이메일 API임.
9.  온프레미스 MongoDB에서 CosmosDB로 마이그레이션하려고 한다. 어떤 전략을 사용할 것인가? Data Management Gateway Tool도 포함할 수 있음.  
    🔔 **mongorestore**  
      > :black_nib: mongorestore imports your BSON file dump into Azure Cosmos DB.
10.  e-commerce Web app 만들려고 하는데 가입하는데 keyVault 사용하고, 이 앱이 azure app service authentication and aad를 사용해서 secured하고 싶다. 뭘 해야할까?  
   🔔 **Enable Managed Service Identity (MSI).**  
      > :black_nib: 관리ID를 부여하여 서비스를 관리하면 AAD protected Rrs를 손쉽게 access 할 수 있음(such as key-vault)
    
