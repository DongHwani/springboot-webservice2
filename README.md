# springboot-webservice2

"스프링 부트와 AWS로 혼자 구현하는 웹 서비스" 책 학습 프로젝트

**학습 목표** : 클라우드 환경에서의 빌드, 배포 싸이클을 학습한다. 


요약 및 느낀점
----
- JPA와 Spring Security에 대한 약간의 지식이 있을 경우, 1장 ~ 5장까지는 반나절이면 완성
- 6장부터 클라우드 환경 실습 시작. EC2 인스턴스 개념 및 생성 후 인바인드 아웃바운드 설정과 보안그룹에 대한
설명과 실습 진행. Management Console로 쉽게 방화벽과 보안그룹을 생성할 수 있음 
- CI/CD를 진행하기전에 우분투 서버에 쉘스크립트를 작성하여 배포 과정을 실습한다. 
- 이전의 배포 프로세스들을 상기하면서 클라우드 환경에서의 CI/CD 프로세스와 비교해보고 책의 내용을 따라치는게
중요하다고 생각함 
- 어플리케션의 빌드 > 배포 싸이클을 얕지만 빠르게 배울 수 있어 좋았음
- Code로 인프라 환경을 구축한다는 말들이 이해가 안갔었는데 travis CI와 CodeDeploy 설정들을 yml 파일로 관리하면서 대략 어떤 의미인지
이해하게 됨 

- Chapter08부터 인프라 중심 내용 시작, 실질적 학습 구간 진행 부분 


학습내용 정리
---
v. Step 01 배포프로세스  
 - Local 개발 완료 > GitHub Push > EC2 GitHub Pull > Test 수행 > 배포  
　　　　　　　　　　　　　　　               <------------ 배포스크립트 -----------> 
 
v. Step 02 배포 프로세스   
 Local 개발 완료 > GitHub Push > Travis CI, Build 및 Test 수행 > CodeDeploy 배포 > AWS EC2 

실습 중 마주했던 오류
---
 - [Travis CI, yml 파일 parse 문제](https://github.com/dhkdhk/TIL/blob/master/ETC/YamlParseError.md)
 
 

