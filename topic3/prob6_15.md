### π― Question 6-15

6. azure blob storage metadata update?
- π metadata.Add("docType", "textDocuments");
- await blob.SetMetadataAsync(metadata);
- await blob.SetPropertiesAsync();

7. λ§€μΌ 2MB μ₯μΉ λ°μ΄ν°λ₯Ό μμ§νλ μλ£¨μ. κ° μ€ν μ΄μλ 1~5κ°μ μ₯μΉκ° μκ³  μ΄ λ°μ΄ν°λ λΈλ‘­ μ μ₯μμ μ μ₯λ¨. ν₯ν μΆκ° λ§€μ₯ μ€ν μμ .
- π Event Grid does not have a capture feature and it does not store data in Blob storage. You need to use Event Hubs as your source and enable capture with Blob storage as your destination.

8. λ·λ· μ±μ΄ vmμ΄ λ°μ΄ν° μ²λ¦¬λ₯Ό λλΌ λλ§λ€ λ©μμ§λ₯Ό λ°κ³ μ νλ€. μμ  μ±μμ μ²λ¦¬λ νμ λ©μμ§λ μ§μλμ§ μλλ€.

9. λΈλ‘­ μ€ν λ¦¬μ§ νλ¦¬λ―Έμ ν°μ΄ μ¬μ©. 3κ°μλ λ°μ΄ν° κ±°μ μ¬μ© μν¨. κ·Έλ¬λ μ¦μ μ¬μ©ν  μ μμ΄μΌν¨. 1λμ΄ μ§λκ±΄ μ¦μ μ¬μ©νμ§ λͺ»ν΄λ λ¨.
- π μΌλ¨ v2λ‘ μκ·Έλ μ΄λ(ν«,μΏ¨,μμΉ΄μ΄λΈ λλ μ μμ.) -> μμΉ΄μ΄λΈλ  λ°μ΄ν°λ€ λ³΅μ¬ν΄μ μμΉ΄μ΄λΈ ν΄λμ λ³΅μ¬νκ³  μ¬κΈ°μ  μ­μ  -> μΏ¨λ‘ λ³κ²½

10. λΆμ° λ°λ² μ μ°κ²°νλ €λ©΄? 
- π this.cosmosClient = new CosmosClient(EndpointUri, PrimaryKey)

11. μ¬λ¬ μ»¨νμ΄λλ‘ λΆν° λλ λ°μ΄ν°λ₯Ό μ μ₯νλ μ€ν λ¦¬μ§ κ³μ . μ μ€ν λ¦¬μ§λ‘ λ³΅μ¬ν΄μΌν¨. μλνλ μ΄λ, μ¬μ©μ μλ ₯ μ΅μν?
- π AzCopy v10 λͺλ Ήμ€ μ νΈλ¦¬ν°λ₯Ό μ¬μ©νμ¬ μ€ν λ¦¬μ§ κ³μ  κ°μ BLOB, λλ ν λ¦¬ λ° μ»¨νμ΄λλ₯Ό λ³΅μ¬ν  μ μμ.

12. κ΄λ¦¬id μ¬μ©νλ μ μ  μ€ν λ¦¬μ§ κ³μ  μ΄μ©νλ μΉμλΉμ€ κ°λ°. secretμΈμ¦ κΈ°λ°μ νμ©νμ§ μμ. μ μ  μΈμ€ν΄μ€ λ©νλ°μ΄ν° μλΉμ€ μλν¬μΈνΈλ§ μ΄μ©. μ‘μΈμ€ ν ν° κ²μνλ μ½λ μμ±.
- π url: 169.254.169.254/metadata/identity/oauth2/token
- DeserializeObject<Dictionary<string, string>>(payload)

13. cosmosDB selectλ¬Έ μνμ ?
- π compositeIndexes -> desceding

14. 6κ° κ³ μλλ‘ κ΅ν΅ κ°μ¬ μμ€ν κ΅¬μΆ, 4κ° λΆμμμ μ¬μ©. κ° λΆμλ μ μ  μΉμ±μ μ¬μ©νλ©°, λͺ¨λ  μΉμ±μ μΈ κ°μ μΈμ€ν΄μ€μ νλμΌλ‘ κ΅¬μΆλ¨. λ°μ΄ν° μ²λ¦¬λ μ΅λν μ§μ°μκ° μ΅λννλ μ΄λ²€νΈ νλΈ?
> π better to know     
μ΄λ²€νΈ κ·Έλ¦¬λμ νλΈ κ·Έλ¦¬κ³  μλΉμ€ λ²μ€ λΉκ΅
![messageService](./image/messageService.png)
- π number of partition? 6
- partition key? highway

15. MSA κ°λ°, λ€μ€ λΈλ aks ν΄λ¬μ€ν°μ λ°°ν¬.
> - reverse proxy capabilities   
> - configurable traffic routing   
> - TLS termination with a custom certificate  
- π deployee solution ? ****helm(k8s ν¨ν€μ§λ§€λμ )**
- view cluster and external ip addressing?  **k8s**
- implement single public ip endpoint that is routed to multiple msa? **ingress controller**