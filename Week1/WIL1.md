# Git 이란?
Git은 버전 관리 및 협업을 위해 사용하는 오픈소스 소프트웨어입니다.

# Git을 사용하는 이유
- 어떤 파일이 수정됐는지
- 누가 수정했는지
- 언제 수정됐는지
- 어떻게 수정됐는지

이것들을 추적하고 원하는 상태의 코드를 사용하기 위해 Git을 사용합니다.

# 파일의 생명주기
- Untracked: 새로 생성된 파일은 Git이 추적하지 않는 상태
- Unmodified: 수정하지 않은 상태
- Modified: 커밋된 파일이나 스테이징 영역에 있는 파일이 수정되면 해당 파일은 수정된 상태로 표시
- Staged: 수정된 파일을 스테이징하여 다음 커밋에 포함할 준비가 된 상태

# Git/GitHub 흐름 정리하기
1. Working Directory: 파일을 수정하고 저장하는 실제 작업 공간. `git add` 명령을 사용하여 수정한 파일을 Staging Area로 올릴 수 있습니다.
2. Staging Area: 커밋할 파일들이 대기하는 곳.
3. Local Repository: 컴퓨터의 로컬 디렉토리에 있는 Git 저장소.
4. Remote Repository: 네트워크 상의 다른 위치에 있는 Git 저장소.

# Git으로 파일 관리하기
1. 디렉토리에 Git 저장소를 만들기
   - `git init`
2. Git으로 관리할 대상 등록하기
   - `git add`
3. 파일 수정 후 로컬 저장소로 옮기기
   - `git commit`
4. 깃허브와 로컬 연결
git remote add origin https://github.com/MinJuune/2024-1-Beginner-Study.git
git branch -M main
git push -u origin main


# 수정할 때
1. 수정한 파일 저장 -> "Modified" 상태
2. `git add .` -> 수정된 모든 파일을 Staging Area로 올림
3. `git commit -m ""` -> Staging Area에 있는 파일들을 커밋하여 로컬 저장소에 변경 사항을 저장
4. `git push origin main` -> 로컬 저장소의 변경 사항을 원격 저장소인 GitHub의 "main" 브랜치에 푸시하여 변경 사항을 업로드


# 실습
 https://github.com/MinJuune/MinJuune/tree/main/MinJuune