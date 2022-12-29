# git flow 관리
## branch 관리
  * branch를 이용해서 독립된 다수의 작업흐름을 관리하고 통합할 수 있음
  * 현업에서 통상 `release branch`는 검수 대상으로 사용됨

## GitHub flow
* `Pull request` 방식을 기반으로 함
### 작업순서 - Shared Repository Model(초대 방식)
* 동일한 저장소를 공유하는 방식
* 초대 받음 -> 수락 ('collaborator'로 등록되어야 `push` 권한이 부여됨)
* 로컬로 복제 (`git clone <url>`)
* 새 branch 만들기 (*원격 저장소 내 독립된 branch에 작업하는 것이 중요*)
  * `git branch <branchname>`
  * 혹은 `git checkout -b <branchname>`: 생성과 checkout 동시에
* 작업 -> `add`, `commit`, `push`
* `Pull Request` 생성
  * 리뷰어, 담당자, label 등 설정할 수 있음
* `merge` 단계
  * `master branch`로 병합하는 경우 배포 가능한 상태인지 확인 필수
### 작업순서 - Fork & Pull Model
* 원격 Project repository를 내 원격저장소로 `fork`
* 로컬로 Clone (`url`에 내 저장소를 입력했는지 확인할 것)
* 작업, `add`, `commit`, `push`
* `Pull Request` 생성