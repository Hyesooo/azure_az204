### ๐ฏ prob1 ~ prob11

1. ๋๊ฐ์ Hiper-v ํธ์คํธ๊ฐ ์๋ค. Host1์ VM1์ ๋ํ๋ก์ด ๋์ด์๋๋ฐ, ์ด๋ฅผ Host2d-์ ์ฎ๊ธฐ๊ธฐ ์ํด ํ  ์ผ์?     
๐ **From th Redeploy blade, click Redelploy**
   > :black_nib: Hiper-v ? ์๋์ฐ ๊ฐ์ํ ํ๋ก๊ทธ๋จ.
   > ์ ํธ์คํธ๋ก ๋ฐ๊พธ๊ณ  ์ถ์ ๊ฒฝ์ฐ ์ฌ ๋ฐฐํฌํ  ๊ฒ.

2. ๋ํ๋ก์ด๋ฅผ ์ํด ARM tamplate์ ๋ค์ด๋ก๋ ๋ฐ์๋ค. ๊ทธ๋ฌ๋ ๋น๋ฒ์ด palin-text์ด๊ธฐ๋๋ฌธ์, administrative password ์ฐธ์กฐ๋ฅผ ์ ์ฉํด์ผํ๋ค. ์ด ๋ ํ  ์ผ์?      
๐ **Azure key valut, Access policy**
   > :black_nib: Using an Access Policy we allow access to the previously created secret.
3. AAD์ joined๋ AKS๋ฅผ ๊ด๋ฆฌ ์ค์ผ ๋, ๊ฐ๋ฐ์๊ฐ myApp์ ์ฌ๊ธฐ์ ๋ฐฐํฌํ๊ณ ์ ํ๋ค. ์ด ์ฑ์ ์ํด YML ๋งค๋ํจ์คํธ ํ์ผ์ deployeeํด์ผํ๋๋ฐ, ์๋ง์ ์ก์์?  
๐ **Azure CLI๋ฅผ ๋ก์ปฌ์ ์ค์น ํ run the kubectl apply f myapp.yaml command**
   > :black_nib: To deploy a YAML file to Kubernetes you need to use the โkubectlโ command 

4.  *same with no.3*  
5. ์๋ก์ด ๋ฐ์ดํฐ๊ฐ ํ์ ๋ค์ด์ฌ๋๋ง๋ค ์ฝ๋์ ํน์  ํจ์๋ฅผ ์ธ๋ณดํฌ ์ํค๋ ์ฑ ์๋น์ค์ ๋ฐฑ๊ทธ๋ผ์ด๋ ํ์คํฌ๋ฅผ ํธ๋ฆฌ๊ฑฐ ํ๋๋ก ๋์์ธ ๋ WebJobs SDK ์ฌ์ฉํ ๋, ํ ์์ดํ๋ค์ ์ฒ๋ฆฌํ๋ ์๋น์ค ๊ตฌ์ฑ์ ํ๋ ค๊ณ ํ๋ค. ์ด๋ ์ฌ์ฉํ  ์๋น์ค๋?  
๐ **WebJobs**  
   > :black_nib: ํน๋ณํ ์ธ๊ธ์ด ์๋ค๋ฉด WebJobs SDK์ ๊ฐ์ฅ ํธํ์ด ์ข์๊ฒ์ webJobs, ๊ทธ๋ฌ๋ Function๊ณผ ๋น๊ตํ์ ๋ ๊ธฐ๋ฅ์ด ์๋๋ ๊ฒ์ด ๋ง์.
   
6. ARM ํฌํ๋ฆฟ์ผ๋ก ์ ์  ๋ฆฌ์์ค๋ฅผ ๋ํ๋ก์ด ํ๊ณ ์ ํ๋ค. VM์ ํ๋์ ๊ฐ์ฉ์ฑ ์งํฉ์ ๊ฐ๊ณ  ์๋ค. ARM ํฌํ๋ฆฟ์ด ์ฅ์  ๋๋ ์ ์ง๋ณด์์์ ๊ฐ๋ฅํ ๋ง์ VM์ ์ ๊ทผ๊ฐ๋ฅํ๊ฒ ์ ์งํ๊ณ  ์ถ๋ค. platformFaultDomainCount์ ์ด๋ค ์ค์ ์ ํ ๊ฒ์ธ๊ฐ?   
   ๐ **Max Value**  
   > :black_nib: Max value for Fault Domain is 3 and Update Domain is 20 in a single availablity set.
   >
   > ์ฅ์ ๋๋ฉ์ธ์ ๋ฌผ๋ฆฌ์  PC๋ฅผ ์๋ฏธํ๊ณ , update๋๋ฉ์ธ์ vmํ๋๋ฅผ ์๋ฏธํจ.

7.  *same with no.6*  
8.  CosmosDB SQL API ์ด์ฉํ๋๋ฐ, Iot ๋๋ฐ์ด์ค์ ์ ๋ณด๊ฐ ๋ค์ด์ค๋ฉด ์ด๋ฉ์ผ์๋ฆผ์ ๋ณด๋ด์ผํ๋ค. (๋น์ฉ ์ ๊ฐ๋ ์ฒดํฌํด์ผํจ.) ์๋ง์ funtion App ์ค์ ์?     
   ๐ **consumption plan, sendGrid binding**     
      > :black_nib: ๋น์ฉ์ ๊ฐ์ํด comsumtion plan ์ฒดํฌํ๊ณ , ์ ์  ํ์์์ ์ด๋ฉ์ผ ๋ณด๋ด๊ธฐ ์ํด์๋ sendGrid ๋ฐ์ธ๋ฉ์ ์ด์ฉํ๋ค. sendGrid API๋ azure์์ ์ฌ์ฉํ๋ ์ด๋ฉ์ผ API์.
9.  ์จํ๋ ๋ฏธ์ค MongoDB์์ CosmosDB๋ก ๋ง์ด๊ทธ๋ ์ด์ํ๋ ค๊ณ  ํ๋ค. ์ด๋ค ์ ๋ต์ ์ฌ์ฉํ  ๊ฒ์ธ๊ฐ? Data Management Gateway Tool๋ ํฌํจํ  ์ ์์.  
    ๐ **mongorestore**  
      > :black_nib: mongorestore imports your BSON file dump into Azure Cosmos DB.
10.  e-commerce Web app ๋ง๋ค๋ ค๊ณ  ํ๋๋ฐ ๊ฐ์ํ๋๋ฐ keyVault ์ฌ์ฉํ๊ณ , ์ด ์ฑ์ด azure app service authentication and aad๋ฅผ ์ฌ์ฉํด์ securedํ๊ณ  ์ถ๋ค. ๋ญ ํด์ผํ ๊น?  
   ๐ **Enable Managed Service Identity (MSI).**  
      > :black_nib: ๊ด๋ฆฌID๋ฅผ ๋ถ์ฌํ์ฌ ์๋น์ค๋ฅผ ๊ด๋ฆฌํ๋ฉด AAD protected Rrs๋ฅผ ์์ฝ๊ฒ access ํ  ์ ์์(such as key-vault)
    
