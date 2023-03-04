### 💯 Question 8-17

8. 애저 app configuration에서 관리하고 있는 닷넷 코어 앱 개발. 내보내기가 포함된 azure app configuration 저장소 생성. 
> 🔖 better to know     
App Configuration? 중앙 통제가 가능.

9. 애저 키볼트이용. AAD 변경사항 최소화.
- 🔔 User assigned MI 

10. 진료기록카드 관리 웹사이트 개발. 저장된 양식을 서드파티에서 다운로드 할 경우 양식 내용이 손상되면 안됨.
- 🔔 키볼트 발급 -> 키볼트로 양식 암호화 -> 암호화된 데이타 블롭 스토리지에 보관
-  Cosmos DB is for semi-structured data, not for unstructured data. 
- not to store "data" in Azure Key Vault.

13. 리눅스 가상머신에 새 앱 디플로이 하려고함. vm이 보안에 지켜져야함. disk암호화 설정?
- 🔔 키볼트 생성 -> 키볼트 키 생성 -> vm생성 -> vm 암호화 enable (volumeType: all)

14. azure api 개발. 타 리소스 접근 위해 인증?
- 🔔 관리ID

15. 두 개 구독 접근가능한 애저 사용자 계정. 스토리지 어카운트 키 시크릿 가져와야함.
- 🔔 구독 조회 후 컨텍스트 세팅 -> 사용할 글로벌 변수 지정 -> 애저 키볼트 시크릿 get

16. vm이 특정한 리소스그룹에만 접근하도록 리소스 매니저 설정하고 싶다. 리소스매니저 액세스 토큰 취득해야함. 
> 🔖 better to know     
Azure Resource Manager
- 🔔 Azure RBAC is an authorization system built on Azure Resource Manager that provides fine-grained access management of Azure resources
