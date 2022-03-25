## 1. 클라이언트 배포 자동화 파이프라인 구축
####  AWS에서 제공하는 서비스를 이용하여 정적 웹 페이지를 자동 배포 및 호스팅하는 파이프라인을 구축

![git issue](https://user-images.githubusercontent.com/75375944/160069562-56f795e0-0c66-482d-b23e-94c90a328ab4.png)
- AWS 개발자 도구 서비스를 이용해서 배포 자동화 파이프라인을 구축해야 합니다.
- CodePipeline을 이용해서 각 단계를 연결하는 파이프라인을 구축합니다.
- Source 단계에서 소스 코드가 저장된 GitHub 리포지토리를 연결합니다.
- Build 단계에서 CodeBuild 서비스를 이용하여 수동으로 진행했던 build 과정을 자동으로 진행합니다.
- Deploy 단계에서 결과물을 S3 버킷에 자동으로 전달합니다.
- 나중에 변경 사항을 GitHub 리포지토리에 반영했을 경우, 배포 과정이 자동으로 진행되어야 합니다.
- 배포 과정에서 오류가 생길 경우, log 파일을 참조하여 문제점을 확인할 수 있어야 합니다.
 
## 2. 서버 배포 자동화 파이프라인 구축
![image](https://user-images.githubusercontent.com/75375944/160078750-424e02f6-df8a-4553-a7c9-29c7cdfbad52.png)
- AWS 개발자 도구 서비스를 이용해서 배포 자동화 파이프라인을 구축
- AWS 개발자 도구 서비스를 이용해서 배포 자동화 파이프라인을 구축해야 합니다.
- CodePipeline을 이용해서 각 단계를 연결하는 파이프라인을 구축합니다.
- Source 단계에서 소스 코드가 저장된 GitHub 리포지토리를 연결합니다.
- Deploy 단계에서 CodeDeploy 서비스를 이용하여 EC2 인스턴스에 변경 사항을 실시간으로 반영합니다.
- 나중에 변경 사항을 GitHub 리포지토리에 반영했을 경우, 배포 과정이 자동으로 진행되어야 합니다.
- 배포 과정에서 오류가 생길 경우, log 파일을 참조하여 문제점을 확인할 수 있어야 합니다.
