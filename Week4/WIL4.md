# 오늘의 토픽
 - 브랜치 전략
 - 개발자로서의 Attitude


## 브랜치 전략

### 브랜치 관리의 필요성
 - 서로의 작업에 영향을 주지 않기 위해 브랜치의 분리 필요
 - 각 브랜치가 어떤 작업을 위해 존재하는지 구분 필요
 - main 브랜치의 안전한 관리 필요

### 브랜치 보호 규칙
- 승인 없이 Pull Request를 병합할 수 없도록 제한 가능
- 특정 브랜치에 Push 가능자를 제한 가능

### 브랜치 전략
브랜치 전략은 두종류가 있는데, Git Flow랑 GitHub Flow가 있다. 

### 브랜치 종류
- Main Branches
  - main(master)
  - develop
- Supporting branches
  - feature
  - release
  - hotfix
   
#### main
- 프로젝트 생성시 기본으로 생성되는 브랜치
- 영원히 존재하는 첫 번째 브랜치
- 병합될 때마다 제품의 새로운 버전이 탄생
- main이라는 이름 대신 master를 사용하기도 함

#### develop
- 영원히 존재하는 두번째 브랜치
- feature 브랜치의 기반이 됨

#### feature
- develop 브랜치에서 분기하여 작업
- 기능 개발 완료 후 다시 develop으로 병합

#### release 
- 배포 준비를 위한 브랜치
- 자잘한 버그를 수정하고 QA 작업을 함
- develop 브랜치에서 분기하여 main 브랜치로 병합

#### hotfix
- 배포 환경에서 즉각적인 수정이 필요할 경우 사용
- main 브랜치에서 분기
- main, develop 모두에 병합 필요

### Git Flow, GitHub Flow
Git Flow는 배포가 수시로 이루어지는 현 시대의 웹앱과는 부적합. 
이를 개선하기 위해 GitHub Flow 고안

## 개발자로서의 Attitude

### Attitude
- convention을 만들어 사용하자
- 구글링을 꼼꼼히 하자
- 코드에 대한 주인 의식을 가지자
- 질문을 잘 하자