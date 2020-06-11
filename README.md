# Playground.IBM-Cloud-Start

IBM Cloud 첫경험

How to deploy

1. IBMCLOUD CLI를 설치한다.
2. 아래 절차에 따라 진행한다.

#### ibmcloud login
 - 로그인을 한다. 가상 Shell로 넘어가 유지하지 않는데 당황할 필요 없다. 성공했으면 로그인 된거다.
 
#### ibmcloud account show
 - 만일 로그인을 하였다면 나의 유저정보가 보일 것이다.
 
#### ibmcloud target -g [RESOURSE_GROUP] 
 - 이제 resource groups를 설정해야 한다. 대부분 IBM 클라우드 경험을 위해 LITE 유저로 실행중일 것인데, 특별한 설정을 하지 않았다면 `Default`일 것
 - 자신이 사용하는 리소스 그룹이름이 궁금하다면 [관리]->[계정]->[계정리소스] 하부에 있는 [리소스 그룹]을 선택하면 된다.
 - 주의! 만일 Cloud Foundry를 이용한다면 2020년 6월 12일 현재 한국 서버에는 없으므로 region을 us-south 등으로 IBM 리소스를 생성할 때 지정했던 위치에 맞춰야 한다. 한국 서버로 하면 인스턴스를 못찾는다.
 
#### 배포할 App 경로로 이동

#### manifest.yaml 편집

#### ibmcloud --cf : cloud foundry
 - IBM Cloud CLI에 Cloud Foundry가 설치되었는지 확인한다.
 
#### ibmcloud cf install
 - IBM Cloud CLI에 Cloud Foundry가 설치
 
#### ibmcloud cf push
 - Deploy
