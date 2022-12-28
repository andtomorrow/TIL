# Git commands

1. git 초기화(.git 생성)
    ```
    $ git init
    ```
2. staging area에 추가
    ```
    $ add .
    ```
    (모든 파일이라면 `.`을, 개별 파일의 경우는 파일이름을 입력)
3. 커밋
    ```
    $ commit -m (메시지)
    ```

# 221228
## 원격저장소 이용하기
- github에서 새 원격저장소 생성
- 로컬저장소에 원격저장소 정보 설정
- `git remote add origin https://github.com/{userid}/{repositoryname}.git`

## commands
* `git push origin master`
* `git pull origin master`

## 원격에 있는 프로젝트를 가져오려면
* `git clone`
    - 협업 프로젝트 참여 등의 경우. commit history 포함하여 전부 복제함
* `git pull`
    - 원격저장소의 master를 가져오기
## 주요 명령어들
* `git clone` <url> : 원격저장소 복제
* `git remote -v` : 원격저장소 정보 확인
* `git remote add` <remote repository name> <url>
* `git push` <remote repository name> <branch>
* `git pull` <remote repository name> <branch>