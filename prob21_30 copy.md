### 💯 prob21 ~ prob30

21. Log Analytics workspace쓰는 데 윈도우 2012 이나 2016을 쓰는 서버들이 연결되어있다. multi-dimensional platform. **이해 X**    
    🔔 **The Metric signal type.**   
      > ✒️Signal types    
      > * Activity Log: includes service health records along with records on any configuration changes made to the resources (and is available to all Azure resources)     
      > * Audit Log: contains the history of sign-in activity and audit trail of changes made within a particular tenant     
      > * Metric: numerical values that are collected at regular intervals and describe some aspect of a system at a particular time

22. 휴가 숙박 제공업체 조사하는 앱 개발, 앱이 관련 문서를 찾기위해 다양한 기준을 사용하여 인덱스를 검색할 수 있도록 azure search를 구현하려고 한다. 고객이 정규식을 사용하여 인덱스 검색하게 하고싶다면?     
    🔔 **Configure the QueryType property of the SearchParameters class..**   
23. *LogicApp is not in the scope*
24. RESTFUL service implementation, API Management service instance에 대한 backend 권한설정 방법? **이해 X**     
    🔔 **basic, client certifcation, managedId**   
      > ✒️ API Management servie authentication policies.
      > Authenticate with Basic - Authenticate with a backend service using Basic authentication. ->
      > Authenticate with client certificate - Authenticate with a backend service using client certificates. ->
      > Authenticate with managed identity - Authenticate with a backend service using a managed identity. -> Azure Resource
25. *same*  
26. *same*  
27. *same*  
28. 휴가 숙박 제공업체 조사하는 앱 개발, 앱이 관련 문서를 찾기위해 다양한 기준을 사용하여 인덱스를 검색할 수 있도록 azure search를 구현하려고 한다. 고객이 특정기준으로 검색하게 하고싶다면?       
    🔔 **configure Filter property of searchParameter class**   
29. *LogicApp is not in the scope*  
30. Azure Search에서 인덱스를 만듭니다. NET SDK를 사용하여 관련 데이터를 Azure Search 서비스로 가져와야 합니다.         
   🔔 **Create SearchIndexClient object to connect to the search index**    
   **Create an indexBatch that contains the doc which must be added**    
   **call th doc.index methods of the searchindexclient and pass the indexbatch**  
